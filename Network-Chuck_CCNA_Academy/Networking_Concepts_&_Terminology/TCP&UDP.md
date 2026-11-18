## TCP & UDP 

1. TCP & UDP are both in the Transport Layer and segment data from the Application Layer, Presentation Layer, and Session Layer. TCP and UDP break data into segments and add port information to the header.
2. <img width="1365" height="378" alt="image" src="https://github.com/user-attachments/assets/605ffec6-e102-492d-8e6e-3c6fa0528964" />
3. <img width="1368" height="199" alt="image" src="https://github.com/user-attachments/assets/a4fcd96f-c006-497a-a896-8ecb5974145a" />

##### TCP Compared to UDP

| Attributes | TCP | UDP | 
| :--------: | :-: | :-: |
| Connection Type | Connection-oriented (requires a formal handshake before sending data). | Connectionless (fires data packets immediately without checking readiness). |
| Reliability | Guarantees delivery; retransmits lost packets and ensures in-order delivery. | No guarantees; packets can be lost, duplicated, or arrive out of order. | 
| Performance | Higher packet overhead due to acknowledgments, flow control, and error checking. | Lightweight header with minimal overhead due to no acknowledgements or flow control. | 
| Error Handling | Extensive checking with automatic retransmission requests for corrupted packets. | Basic checksum for error detection, but corrupted or missing packets are dropped. | 
| Applications Services | Web browsing (HTTP/HTTPS), file transfers (FTP), email (SMTP), secure shell (SSH). | Live streaming (video/audio), online multiplayer gaming, DNS lookups, VoIP. | 

###### Socket Pairs 

- Source and destination ports are placed within the segment. The segment is encapsulated within the IP packet. The IP packet contains the source and destination address. The combination of the IP address and ports is known as a socket pair.  

#### Port Numbers 

1. <img width="1024" height="559" alt="image" src="https://github.com/user-attachments/assets/4e32ee94-57a2-4182-a368-9b34d7a29b6f" />
2. **Well-Known Ports:** Destination ports used for common application services such as DNS, DHCP, and HTTP, ports ranging from **1** to **1023**.
3. **Registered Ports:** Ports ranging from **1024** to **49151** can be used as source or destination ports. Organizations register specific ports for certain applications.
4. **Private Ports:** Ports ranging from **49152** to **65535** are commonly used for source ports and can be used for any applications.

| Port Number | Transport | Application Protocol | 
| :---------: | :-------: | :------------------: | 
| 20          | TCP       | File Transfer Protocol (FTP) data | 
| 21          | TCP       | File Transfer Protocol (FTP) Control | 
| 22          | TCP       | Secure-Shell (SSH) | 
| 23          | TCP       | Telnet (Note: Insecure) |
| 25          | TCP       | Simple Mail Transfer Protocol (SMTP) | 
| 53          | UDP, TCP  | Domain Name System (DNS) | 
| 67          | UDP       | Dynamic Host Configuration Protocol/BootP (DHCP) Server | 
| 68          | UDP       | Dynamic Host Configuration Protocol/BootP (DHCP) Client | 
| 69          | UDP       | Trivial File Transfer Protocol (TFTP) | 
| 80          | TCP       | Hypertext Transfer Protocol (HTTP) | 
| 110         | TCP       | Post Office Protocol Version 3 (POP3) | 
| 143         | TCP       | Internet Message Access Protocol (IMAP) | 
| 161         | UDP       | Simple Network Management Protocol (SNMP) | 
| 443         | TCP       | Hypertext Transfer Protocol Secure (HTTPS) |

   
