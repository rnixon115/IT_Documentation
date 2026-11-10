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
   -  Fast Recall: If you visit a website commonly, the device checks it local cache first. If the FQDN IP address is saved, the client doesn't send a request DNS Server and the web address loads faster.
   -  Expiration (Time-to-Live or TTL): DNS cache isn't permanent. Time-To-Live (TTL) has a limit, and after time-to-live (TTL) expires, your computer deletes the stored address and ask the DNS Server again.
 




- DHCP uses D.O.R.A or Discover-Offer-Request-Acknowledge process.
   1. **DISCOVER, PORT(UDP 67, SERVER), BROADCAST:** A DHCP Client will send out a Discover message for the DHCP server on the network. Since the client doesn't know the DHCP server's IP address, it broadcasts 255.255.255.255. The DHCP client broadcasts on the network and broadcasts on the data link layer. 
       - DHCP Client: Source_IP: 0.0.0.0, Destination_IP: 255.255.255.255, Src_MAC_Addr: DHCP Client's MAC Address, Dst_MAC_Addr: FF:FF:FF:FF:FF:FF;
   2. **OFFER, PORT(UDP 68, CLIENT), UNICAST:** The DHCP server receives the Discover message from the client and relays a DHCP offer request to the client with information. The DHCP Client still doesn't have an IP address. The DHCP server broadcasts at the network layer, and the data link layer is unicast. 
       - DHCP Server: Source_IP: IP Address of The DHCP Server, Destination_Address: 255.255.255.255, Src_MAC_Addr: DHCP Server's MAC address, Dst_MAC_Addr: MAC address of the DHCP Client;
   3. **REQUEST, PORT(UDP 68, SERVER), BROADCAST:** The DHCP client receives the Offer message and sends back a Request message to the DHCP server. The message tells the DHCP server the client accepts the IP address. The destination address is 255.255.255.255 because there may be one DHCP server or there's a DHCP relay server.
        - DHCP Client: Source_IP: 0.0.0.0, Dst_IP_Source: 255.255.255.255, Src_MAC_Addr: DHCP Client's MAC address, Dst_MAC_Addr: DHCP Server's MAC address;
   4. **ACKNOWLEDGE, PORT(UDP 67, CLIENT), BROADCAST:** At the end of setting up the DHCP Client on the network, the DHCP server broadcasts a message to confirm the lease of the IP address and settings to the client. The acknowledgement indicates the DHCP client can set up its network interface with the provided information. DHCP ACK message is essential because it tells the DHCP Client it can now use the IP address.
        - DHCP Client: Source_IP: Assigned IP address, Destination_IP: 255.255.255.255, Src_MAC_Addr: DHCP Client's MAC address, Dst_MAC_Addr: DHCP Server's MAC address;
