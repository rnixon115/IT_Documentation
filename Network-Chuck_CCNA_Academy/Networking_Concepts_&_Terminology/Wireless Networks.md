## Wireless Networks 

##### Wireless Technologies 

- Wireless technology is composed of unlicensed radio waves in the electromagnetic spectrum. <img width="1665" height="240" alt="image" src="https://github.com/user-attachments/assets/50905d55-3d23-4ff7-8af7-c18f59e224f7" />
- The Wireless Fidelity (802.11) standard was created by the Institute of Electrical and Electronics Engineers; the organization is responsible for networking standards. The organization was founded in February 1980, which led to the creation of the 802 (year, month). 802.11 is the standard number for wireless local area network technologies.


###### 802.11 Standard

1. The 802.11 standard defines how radio frequencies are used for wireless links. 802.11 standards commonly specify how one antenna transmits and receives wireless frequencies on 2.4GHz or 5GHz.
2. Newer standards have been published to provide better performance by increasing speed and using Multiple-Input, Multiple-Output (MIMO) technology. MIMO requires the devices to have both input and output antennas to perform efficiently. Also, MIMO can use up to 8 transmitters or receivers to increase throughput.

| IEEE Wireless Standard | Radio Frequency | Description |
| :--------------------: | :-------------: | :---------: |
| 802.11                 | 2.4 GHz         | Speed of up to 2 Mbps | 
| 802.11a                | 5 GHz           | Speed of up to 54 Mbps, small coverage area, less effective at penetrating building structures, and not interoperable with 802.11b and 802.11g  | 
| 802.11b                | 2.4 GHz         | Speed of up to 11 Mbps, longer range than 802.11a, and better at seeping through buildings | 
| 802.11g                | 2.4 GHz         | Speeds of up to 54 Mbps, backward compatible with 802.11b, and reduced bandwidth |
| 802.11n                | 2.4 GHz & 5 GHz | Transmission rates from 150 Mbps to 600 Mbps with a distance of 70m (230 feet), AP's and client devices requiring multiple antennas for Multiple-Input, Multiple-Output technology |
| 802.11ac               | 5 GHz           | Transmission rate from 450 Mbps to 1.3 Gbps (1300 Mbps), use up to eight antennas; backward compatible with 802.11a/n devices, with limited data rates |
| 802.11ax               | 2.4 GHz & 5 GHz | Also known as Wi-Fi 6 or High-Efficiency Wireless (HEW), improved power efficiency, higher transmission rates, increased capacity, and handles many connected devices; will use 2.4 GHz, 5 GHz, or 1 GHz to 7 GHz when available; Wi-Fi 6E adds 6 GHz band to assist throughput in dense Wi-Fi areas |
| 802.11be               | 2.4 GHz, 5 GHz, & 6 GHz | Also known as Wi-Fi 7 or Extremely High Throughput (EHT), delivers low latency, faster speeds, and reliability for AR/VR or 8K video | 

#### WLAN Components

1. End device with the capability to connect to Wi-Fi with a transmitter and a receiver.
2. Wireless Network Interface Card.
3. If a device doesn't have an integrated Wireless NIC, then a USB wireless adapter is needed.
4. Many devices such as Smartphones, Tablets, Laptops, smart thermostats, etc have a built-in Wireless antenna.
5. An access point provides the 802.11 standard.
6. A switch provides ports for wired LAN devices.
7. A router provides access to other networks.

##### Wireless Settings

<img width="624" height="520" alt="image" src="https://github.com/user-attachments/assets/6db4f7dc-49df-4a59-a6d6-251aea7733a7" />

- Network Mode determines the technology standard being used. Devices that comply with the 802.11 AP standard can achieve maximum transmission speed. If the AP is set up with only one mode, devices must be able to connect to that specific mode. One Service Set Identifier maps to a VLAN in an office environment. Also, several AP's can have the same SSID depending on how they're configured. 
- Network Name (SSID): Is used to identify the Wi-Fi so that end devices can connect to the Wi-Fi. SSID stands for Service Set Identifier.
- Network Broadcast: The AP broadcasts the SSID to nearby devices. Broadcasting the name has been disabled; client devices must enter it manually. Tip: Even disabling the broadcast will not make it secure; ensure the AP uses the strongest encryption and change the default password.
- Channel Settings: The channel settings refer to which frequency band to use when transmitting wireless data. Wireless routers and Access Points can scan the radio frequency channels and select a channel setting automatically. You can manually set the channel if there's interference.
- Security Mode: Security mode refers to the security parameter, and the security parameter can be WEP, WPA, WPA-2, WPA-3, etc.

##### AP Categories 

- An Autonomous AP is a standalone device that is set up in a SOHO setup, small office, or organizational event. Typically, you can set up an autonomous AP via a GUI or CLI interface, and it doesn't need to be managed by a centralized system. 
- <img width="653" height="470" alt="image" src="https://github.com/user-attachments/assets/ccc83e61-52e5-45d2-99c3-62892ee4a0e5" />
- A Controller-Based AP is a centralized system that controls APs in an office or campus-wide area. Each AP is a lightweight AP (LAP) because it uses the Lightweight Access Point Protocol (LWAPP) to communicate with a WLAN Controller (WLC). The WLAN Controller automatically manages and configures each AP in a network.
- <img width="788" height="663" alt="image" src="https://github.com/user-attachments/assets/1e2a1136-bad8-4558-a203-e0d628c87819" />
- Example: [TP-Link Omada APs](https://www.omadanetworks.com/us/landing/omada-access-point/)

##### Common Problems & Solutions to WLAN 

1. Range and Coverage Problems:
   - Problem: WLAN has a limited coverage area. Devices that are too far from the router will experience latency and lose connection.
   - Solution: To resolve the issue, it's best to set up repeaters or a wireless mesh network to expand coverage.
2. Bandwidth Bottlenecks:
   - Problem: Too many devices connected to the same WLAN, and network congestion leads to slow data speeds.
   - Solution: Upgrade the current WLAN or add more AP's. When expanding, make sure that the channels do not overlap.
3. Compatibility Issues:
   - Problem: Modern wireless routers have a higher standard, making it harder for older wireless technologies to connect.
   - Solution: Check the online manual of the wireless router to see if there's an option to support old standards. If that option isn't available, go buy a wireless router that can support older wireless standards.
     
  


