## DNS, DHCP, HTTP

#### Domain Name System (DNS)

- The Domain Name System is the World Wide Web phonebook. On the internet, Fully Qualified Domain Names (FQDNs), such as https://www.google.com, are much easier to remember than 201.145.32.12.
- DNS lookup is a 5-step Process:
     1. Type the name of the FQDN's web address.
     2. A DNS Lookup query is sent to the corresponding DNS server.
        - <img width="1189" height="473" alt="image" src="https://github.com/user-attachments/assets/c5714406-fcfd-4a00-a0a9-f53ab7ecfbec" />
     3. The DNS Server matches the FQDN with its IP address.
        - <img width="1241" height="506" alt="image" src="https://github.com/user-attachments/assets/67219a3d-3a20-4343-8d12-b481d4db8da9" />
     4. The DNS Server sends the client the IP address of the FQDN server.
        - <img width="1194" height="480" alt="image" src="https://github.com/user-attachments/assets/df9c1cf3-e4ac-4f93-9db3-c801f8355fe7" />
     5. The client uses the IP address to request the server.
        - <img width="1213" height="491" alt="image" src="https://github.com/user-attachments/assets/ac4cb323-0741-4716-9ce3-d9eaeceb94d5" />

- **DNS Caching**
   -  Initial Query: The client will request the IP address associated with the FQDN from the DNS server. Once the DNS Server sends back the FQDN IP address to the client, they'll store or cache the results into their computer.
   -  Fast Recall: If you visit a website commonly, the device checks its local cache first. If the FQDN IP address is saved, the client doesn't send a request to the DNS server, and the web address loads faster.
   -  Expiration (Time-to-Live or TTL): DNS cache isn't permanent. Time-To-Live (TTL) has a limit, and after the time-to-live (TTL) expires, your computer deletes the stored address and asks the DNS Server again.

### Automatic IP Address Assignment

- **Windows IPv4 APIPA:**
    1. Windows OS's can automatically generate an IPv4 address using APIPA (Automatic Private IP Addressing). APIPA assigns an address from 169.254.0.1 to      169.254.255.254 when no static address is set and the DHCP Server doesn't respond. APIPA provides LAN connectivity but no internet connectivity.
- **IPv6 LLA:**
    1. IPv6-enabled devices must have a Link-Local Address. If the IPv6 address doesn't have an LLA, then we'll have to configure it manually on the interface. Link-Local Addresses will be created without a DHCP server, and the IPv6 Link-Local Address range is fe80::/10.
- **IPv6 SLAAC:**
    1. IPv6 Stateless Address Autoconfiguration (SLAAC) is a routable address and is automatically assigned by the host. The host configures the address by receiving the network prefix advertised by routers on the network segment and attaching their own unique identifier (typically the MAC address of the network interface card).
 - **Auto Configuration Issues:**
    1. Duplicate Address Conflicts: Autoconfiguration relies on devices sensing and identifying addresses in use on the network. If an error occurs when assigning an address automatically, it usually means the device tries to attach an address that's already in use.
    2. APIPA Limitation: APIPA is great for devices that want to network locally but cannot connect to the internet.
       - Examples: tethering, Bluetooth, hotspot (if no internet access), etc.
    3.  IPv6 SLAAC Issues: IPv6 SLAAC relies on the network broadcast to identify the network prefix. A device may misconfigure IPv6 SLAAC, which causes it to lose connectivity.
#### DHCP 
- Note: When it comes to home routers, they're an DHCP client and a DHCP server. The ISP provides internet and addressing, while the router provides an interface for the Local Area Network. 
- **DHCP uses D.O.R.A or Discover-Offer-Request-Acknowledge process.**
   1. **DISCOVER, PORT(CLIENT SRC_UDP 68, SERVER DST_UDP 67), BROADCAST:** A DHCP Client will send out a Discover message for the DHCP server on the network. Since the client doesn't know the DHCP server's IP address, it broadcasts 255.255.255.255. The DHCP client broadcasts on the network and broadcasts on the data link layer. 
       - DHCP Client: Source_IP: 0.0.0.0, Destination_IP: 255.255.255.255, Src_MAC_Addr: DHCP Client's MAC Address, Dst_MAC_Addr: FF:FF:FF:FF:FF:FF;
   2. **OFFER, PORT(SERVER SRC_UDP 67, CLIENT DST_UDP 68), UNICAST:** The DHCP server receives the Discover message from the client and relays a DHCP offer request to the client with information. The DHCP Client still doesn't have an IP address. The DHCP server broadcasts at the network layer, and the data link layer unicasts. 
       - DHCP Server: Source_IP: IP Address of The DHCP Server, Destination_Address: 255.255.255.255, Src_MAC_Addr: DHCP Server's MAC address, Dst_MAC_Addr: MAC address of the DHCP Client;
   3. **REQUEST, PORT(CLIENT SRC_UDP 68, SERVER DST_UDP 67), BROADCAST:** The DHCP client receives the Offer message and sends back a Request message to the DHCP server. The message tells the DHCP server the client accepts the IP address. The destination address is 255.255.255.255 because there may be one DHCP server or there's a DHCP relay server.
        - DHCP Client: Source_IP: 0.0.0.0, Dst_IP_Source: 255.255.255.255, Src_MAC_Addr: DHCP Client's MAC address, Dst_MAC_Addr: DHCP Server's MAC address;
   4. **ACKNOWLEDGE, PORT(SERVER SRC_UDP 67, CLIENT DST_UDP 68), UNICAST:** At the end of setting up the DHCP Client on the network, the DHCP server broadcasts a message to confirm the lease of the IP address and settings to the client. The acknowledgement indicates the DHCP client can set up its network interface with the provided information. DHCP ACK message is essential because it tells the DHCP Client it can now use the IP address.
        - DHCP Client: Source_IP: Assigned IP address, Destination_IP: 255.255.255.255, Src_MAC_Addr: DHCP Client's MAC address, Dst_MAC_Addr: DHCP Server's MAC address;
<img width="1280" height="568" alt="image" src="https://github.com/user-attachments/assets/f2ecfa1a-2e4d-42ad-a27c-3e3d2dda51fc" />

#### DHCPv6 

1. **DHCPv6 with SLAAC:**
   - A router can be configured to respond to router solicitation (RS) messages with router advertisements (RA) with SLAAC. 
        1. A Client will send a router solicitation message to all IPv6 routers.
        2. The router will send out a router advertisement message to all IPv6 nodes with SLAAC and DHCPv6. The router advertisement response includes the prefix, prefix length, and default gateway. DNS information will come from the DHCPv6 server.
        3. T
The PC sends a DHCPv6 Solicit message to all DHCPv6 servers. "I used SLAAC to create my IPv6 address and get my default gateway address, but I need other information from a stateless DHCPv6 server."

