# Physical Layer
The physical layer consists of physical media to *connect* to other devices.
1. Ethernet Cables
2. Fiber
3. Wireless
4. Satellite
5. Cellular
   
### The phyiscal layer is about the *hardware instead of software*, so, problems can consist of:
1. Fixing cables / replacing cables
2. Crimping
3. Punching down
4. Running loopback test
5. Swapping Network Interface cards
6. etc

### Bit synchronization 
- Bit synchronization is important because both the sender and receiver need to stay in time with each other,
so that the receiver knows when each bit begins and ends.

### Bandwidth and Throughput
- Bandwidth: Refers to the capacity of data that can be transmitted at a time.
- Throughput: Refers to how fast data is being transmitted successfully to the receiver. ( 1 Mbps = 1,000,000 bits per second)  
  
### Physical Topologies 
- Physical Topologies are how to define networking devices in a structure. ( Star, Mesh, Bus, Ring )
- ![Physical Topologies](https://encrypted-tbn2.gstatic.com/licensed-image?q=tbn:ANd9GcSKow8-GZBrZSMX4Ii5yZP5FgnKKf1o-ejwgSRCsjNKfEL_rtyvHnkPpf4iN2Q8X6RxOYh5NOo8CG57ha3_1FzJ0KP6PSe8GOjZwrs5QW-IY297ppE)

### Physical Layer Standards & Protocols 
- IEEE (Institute of Electrical and Electronics Engineers) 802.3 (**Ethernet**): 802.3 is the standard for wired Ethernet.
- RS-232: Is a standard serial communication interface
- USB (Universal Serial Bus): Is a standard for modern computer peripheral connections.
- EIA (Electronics Industries Alliance)/TIA (Telecommunication Industry Alliance)-232, 449, 530: Standards defining electrical characteristics for data communication equipment.
- DSL (Digital Subscriber Line), ISDN (Integrated Services Digital Network), T1/E1 (T1 & E1 are phone lines. T1 in North America and E1 in Europe): Standards for various types of telecommunication carrier lines.

### Switch Vs a Hub
| Feature | Hub |   Switch  |
| ----------- | ----------- | ----------- |
| OSI-Layer | Physical-Layer | Data-Link Layer |
| Data Unit Handling | Raw Bits | Frames |
| Traffic Forwarding | Broadcasting (All) | Unicasting (Single) |
| Collision Domain | Single large domain for all ports | Separate domain for each port |
| Mode | Half-Duplex (Means 1-way) | Full-Duplex (Both Ways) |
| Intelligence | A Simple Repeater | Remembers MAC Addresses
