# Networking

1. **What is Network?**
   - A network consists of two or more computers that are linked in order to share resources (such as printers, CD), exchange files, or allow electronics communications. The computers on networks may be linked through cables, telephone lines, radio waves, satellites, or infrared light beams.

2. **Why do we need Network?**
   - In the past, data sharing required physical devices like floppy disks or USBs, and each computer needed its own printer. This approach was slow, costly, hard to manage, and didn’t scale. As data and collaboration needs grew, it became inefficient.
Networks solved these problems by enabling fast, reliable, and scalable digital communication, allowing devices to share resources and data seamlessly.

3. **Network Protocol**
   - A protocol is a set of rules for formatting and processing data. A network protocol (e.g. TCP/IP) is a set of rules that define how data is formatted, transmitted, and processed across a network.
It acts like a common language for computers, allowing devices with different hardware and software to communicate seamlessly. By following the same protocol, systems can understand and exchange data reliably, regardless of their internal differences.

4. **Why do we need Network Protocols?**
   - In the early days, organizations created their own proprietary protocols, which led to isolated systems that couldn’t communicate with each other. This caused major compatibility and communication issues. To solve this, standardized network protocols(e.g. TCP/IP) were developed, allowing different systems to connect and communicate reliably. This shift enabled global interoperability, scalability, and the growth of the internet.

5. **Data Link**
   - A data link is a term used to describe the connection between two systems in order to share the information. A wired data link is a communication method that sends the information over wires or cables. The variations of this type connection are twisted pair cables, coaxial cables, fiber-optic cables and ethernet over copper.

6. **What is Internet?**
   - The internet is a global network of interconnected networks, comprised of clients, servers, routers, and other infrastructure, connected through various means such as cables, wireless connections, and satellite links, all communicating using standard protocols.

7. **Client**
   - A machine or process that requests data or service from a server. Example - Web browsers (Chrome, Firefox, Safari), Mobile App, Email clients (Outlook, Gmail app), etc. Note that a single machine or a piece of software can be both a client and server at the same time. For instance, a single machine could act as a server for end users and a client for a database.
     
8. **Server**
   - A machine or process that provides data or service to a client, usually by listening for incoming network calls. Example - Web servers (Apache, Nginx) that host websites, Email servers (Exchange, Sendmail) that manage email, Database servers (MySQL, PostgreSQL) that store and manage data, etc. Note that a single machine or a piece of software can be both a client and server at the same time. For instance, a single machine could act as a server for end users and a client for a database.

9. **Client Server Model**
   - The paradigm by which modern systems are designed, which consists of clients requesting data or service from servers and servers providing data or service to clients.
  
10. **Internet Protocol**
    - This network protocol outlines how almost all machine-to-machine should be happen to this world. This is the fundamental "language" and addressing system that allows devices to find and communicate with each other. Other protocols are like TCP, UDP and HTTP are built on top of IP.
   
11. **IP Address**
    - An address given to each machine connected to the public internet. IPv4 addresses are consists of four numbers separated by dots: a.b.c.d where all four numbers are between 0 to 255. Special values include: a) 127.0.0.1 Localhost (your own machine) b) 192.168.x.y Private network (e.g., your home Wi-Fi network). IPv6 addresses are eight groups of four hexadecimal digits, separated by colons (e.g., 2001:0db8:85a3:0000:0000:8a2e:0370:7334).
    - IP addresses are essential for identifying and locating devices on the internet. IPv4 is the older version with limited addresses, while IPv6 is the newer version designed to support many more devices.
   
12. **TCP**
    - Network protocol built on top of the Internet Protocol(IP). Allows for ordered, reliable data delivery between machines over public internet by creating a connection. Establishes a connection before data transfer. TCP is usally implemented in the kernel, which exposes sockets to applications that they can use to stream the data through an open connection.

13. **Port**
   - In order for multiple programs to listen for new network connections on the same machine without colliding, they pick a port to listen on. A port is an integer between 0 and 65,535(2^16 ports total).
   - Typically, ports 0-1023 are reserved for system ports(also called well-known ports) and shouldn't be used by user-level processes. Certain ports have pre-defined uses, and although you usually won't be required to have them memorized, they can sometimes come in handy. Below are some examples:
   a. 22: Secure Shell
   b. 53: DNS lookup
   c. 80: HTTP
   d. 443: HTTPS

14. **ISP**
   - An Internet service provider, provides services for accessing, using , or participating in the Internet. ISPs can be organized in various forms, such as commercial, community-owned, non-profit, or otherwise privately owned. The two main types of ISPs are cable or DSL.

15. **HTTP**
   - The Hyper Text Transfer Protocol is a very common network protocol implemented on top of TCP. Clients make HTTp requests, and servers respond with a response. 
   Requests typically have the following schema:
   ```bash
   host: string (example: algoexpert.io)
   port: integer (example: 80 or 443)
   method: string (example: GET, PUT, POSY, DELETE, OPTIONS or PATCH)
   headers: pair list (example: "content-Type" -> 1238)
   body: opaque sequence of bytes
   ```
   Responses typically have the following schema:
   ```bash
   status code: integer (example: 200, 401)
   headers: pair list (example: "content-Type" -> 1238)
   body: opaque sequence of bytes
   ```

16. **HTTPS**
   - The Hyper Text Transfer Protocol Secure is an extension of HTTP that's used for secure communication online. It requires servers to have trusted certificates (usually SSL certificates) and uses the Transport Layer Security(TLS), a security protocol built on top of TCP, to encrypt data communicated between a client and a server.

17. **DNS**
   - Short for Domain Name System, it describes the entities and protocols involved in the translation from domain names to IP Addresses. Typically, machines make a DNS query to a well known entity which is responsible for returning the IP address(or multiple ones) of the requested domain name in the response.

18. **Latency**
   - The time it takes for a certain operation to complete in a system. Most often this measure is a time duration, like milliseconds or seconds. You should know these orders of magnitude:
      - **Reading 1 MB from RAM**: 0.25 ms
      - **Reading 1 MB from SSD**: 1 ms
      - **Transfer 1 MB over Network**: 10 ms
      - **Reading 1 MB from HDD**: 20 ms
      - **Inter-Continental Round Trip**: 150 ms
   
19. **Throughput**
   - The number of operations that a system can handle properly per time unit. For instance the throughput of a server can often be measured in requests per second (RPS or QPS).

20. **Round Trip Time**
   - Round trip time (RTT) is the measure (in milliseconds) of the latency of a network X 2- that is, the time between initiating a network request ( a signal to be sent) plus the amount of time it takes for acknowledgement of that signal having been received (receiving a response). This time delay includes propagation times for the paths between the two endpoints. Simply put, it refers to the time taken by a network request to reach a destination and to revert back to the original source. RTT is a crucial tool in determining the health of a network and can be analysed and determined by pinging a certain address.

21. **Bandwidth**
   - The maximum amount of data transmitted over an internet connection in a given amount of time - calculated in megabits per second (Mbps). Note that bandwidth measures volume not speed.

22. **Cache**
   - A piece of hardware or software that stores data, typically meant to retrieve that data faster than otherwise.
   Caches are often used to store responses to network requests as well as results of computationally-long operations.
   Note that data in a cache can become stale if the main source of truth for that data (i.e., the main database behind the cache) gets updated and the cache doesn't.

23. **Cache Hit**
   - When requested data is found in a cache.

24. **Cache Miss**
   - When requested data could have been found in a cache but isn't. This is typically used to refer to a negative consequence of a system failure or of a poor design choice. For example: 
   If a server goes down, our load balancer will have to forward requests to a new server, which will result in cache misses.

25. **Cache Eviction Policy**
   - The policy by which values get evicted or removed from a cache. Popular cache eviction policies include LRU (least-recently used), FIFO (first in first out), and LFU (least-frequently used).

26. **Ethernet**
   - Ethernet is the traditional technology for connecting devices in a wired local area network (LAN) or wide area network (WAN). It enables devices to communicate with each other via a protocol, which is a set of rules or common network language.

27. **TCP Connection**
   - Transmission Control Protocol (TCP) is a connection-oriented communications protocol that facilitates the exchange of messages between computing devices in a network. It is the most common protocol in networks that use the Internet Protocol (IP), together they are sometimes referred to as TCP/IP.

28. **MAC Address**
   - MAC Address (Media Access Control Address) is a unique identifier assigned to a network interface card (NIC) or other network hardware devices. It is a 48-bit (6-byte) hexadecimal number, typically represented in the format XX:XX:XX:XX:XX:XX, where each pair of characters represents an octet (8 bits). MAC addresses are used at the Data Link Layer (Layer 2) of the OSI Model to enable communication between devices on the same network segment. They ensure that data packets are delivered to the correct destination hardware within a local area network (LAN), enabling devices to distinguish one another at the physical level.
29. **LLC**
   - LLC (Logical Link Control) is a sublayer of the Data Link Layer (Layer 2) in the OSI Model, responsible for managing communication between network devices. The LLC sublayer provides a common interface for various Data Link Layer protocols and allows multiple higher-layer protocols to coexist on the same link. It is responsible for error and flow control, as well as multiplexing and demultiplexing data streams from different sources. The LLC sublayer uses Service Access Points (SAPs) to identify the type of protocol being transmitted and to provide a communication path between the higher-level network protocols and the lower-level MAC sublayer.

30. **OSI Model**
   - OSI Model (Open Systems Interconnection Model) is a conceptual framework that standardizes the functions of a telecommunication or computing system into seven distinct layers. This model was developed by the International Organization for Standardization (ISO) to facilitate communication between different systems and protocols. Each layer performs a specific function in the process of transmitting data between network devices, providing a modular approach to understanding network communication. The seven layers of the OSI Model are:
      - **Physical Layer (Layer 1)**: This layer is responsible for the physical connection between devices, including the transmission of raw bitstreams over a physical medium. It encompasses the electrical, mechanical, and functional specifications of the hardware, such as cables, switches, and network interface cards (NICs).
      - **Data Link Layer (Layer 2)**: This layer provides error-free data transfer between adjacent network nodes by establishing, maintaining, and terminating a reliable link. It is responsible for creating and managing frames, as well as handling flow control, error detection, and correction. The Data Link Layer is divided into two sublayers: the Logical Link Control (LLC) and the Media Access Control (MAC).
      - **Network Layer (Layer 3)**: This layer manages the routing of data packets between devices across multiple networks. It is responsible for determining the best path for data transmission, handling packet fragmentation and reassembly, and managing network congestion. Key protocols in this layer include the Internet Protocol (IP) and Internet Control Message Protocol (ICMP).
      - **Transport Layer (Layer 4)**: This layer is responsible for providing reliable and efficient data transmission between devices, ensuring data integrity and error recovery. It manages end-to-end connections, flow control, and congestion control. Two primary protocols in this layer are the Transmission Control Protocol (TCP) and User Datagram Protocol (UDP).
      - **Session Layer (Layer 5)**: This layer is responsible for establishing, maintaining, and terminating connections between applications on different devices. It manages session setup, synchronization, and teardown, allowing multiple applications to communicate simultaneously over the same network connection.
      - **Presentation Layer (Layer 6)**: This layer handles data translation, formatting, and encryption for proper communication between applications. It is responsible for ensuring that data is represented in a format that can be understood by both the sender and receiver, as well as compressing and decompressing data, if necessary.
      - **Application Layer (Layer 7)**: This layer provides the interface between the user and the network, allowing applications to access network services. It is responsible for various high-level functions, including authentication, file transfer, email, and web browsing. Common protocols in this layer include HTTP, FTP, SMTP, and DNS.

31. **TCP/IP Model**
   - The TCP/IP model is a conceptual framework for understanding and describing how data communications take place between computing systems in the Internet. TCP/IP stands for Transmission Control Protocol/Internet Protocol and is a suite of communication protocols used to interconnect network devices on the internet. TCP/IP is also used as a communications protocol in a private computer network (an intranet or extranet). It is composed of four layers, each representing a different aspect of the communication process. The layers are: network access, internet, transport, and application. The TCP/IP model provides a standard for communication protocols and allows different systems to communicate with each other over the Internet. The four layers of the TCP/IP Model are:
      - **Link Layer (corresponds to OSI Layers 1 and 2)**: This layer is responsible for the physical and logical connections between network devices. It covers the hardware and protocols used to transfer data between adjacent network nodes, including cables, switches, network interface cards (NICs), and protocols such as Ethernet and Wi-Fi.
      - **Internet Layer (corresponds to OSI Layer 3)**: This layer is responsible for the routing and forwarding of data packets between devices across multiple networks. It defines the addressing scheme (IP addresses) and protocols used to transmit data over the Internet. Key protocols in this layer include the Internet Protocol (IP), Address Resolution Protocol (ARP), and Internet Control Message Protocol (ICMP).
      - **Transport Layer (corresponds to OSI Layer 4)**: This layer is responsible for providing reliable and efficient data transmission between devices, ensuring data integrity and error recovery. It manages end- to-end connections, flow control, and congestion control. Two primary protocols in this layer are the Transmission Control Protocol (TCP) and User Datagram Protocol (UDP).
      - **Application Layer (corresponds to OSI Layers 5, 6, and 7)**: This layer provides the interface between the user and the network, allowing applications to access network services. It is responsible for various high- level functions, including authentication, file transfer, email, and web browsing. Common protocols in this layer include HTTP, FTP, SMTP, and DNS.

32. **Encapsulation**
   - Encapsulation is the process of adding additional information when data is traveling in TCP/IP model. When data moves from upper layer to lower layer of TCP/IP protocol stack, during an outgoing transmission, each layer includes a bundle of relevant information called "header" along with the actual data.

33. **Decapsulation**
   - Decapsulation is the process of opening up encapsulated data that are usually sent in the form of packets over a communication network. It can be literally defined as the process of opening a capsule, which, in this case, refers to encapsulated or wrapped-up data.

34. **Private IP**
   - A private IP address is a range of non-internet facing IP addresses used in an internal network. Private IP addresses are provided by network devices, such as routers, using network address translation. If you want to find the IP of a device you're connected to, you can use the "netstat -an" command in the terminal.

35. **Public IP**
   - A public IP address is an IP address that your home or business router receives from your ISP and it's used when you access the internet. Public IP addresses are required for any publicly accessible network hardware such as a home router and the servers that host websites. You can find you public IP address by typing what is my IP on google.

36. **Firewall**
   - A firewall is a network security device that monitors incoming and outgoing network traffic and permits or blocks data packets based on a set of security rules. Its purpose is to establish a barrier between your internal network and incoming traffic from external sources (such as the internet) in order to block malicious traffic like viruses and hackers.

37. **Three Way Handshake**
   - TCP 3-way handshake, also known as a 3-way handshake, is a protocol for establishing a connection between a server and a client in a TCP/IP network. Before the real data communication process begins, both the client and server must exchange synchronization and acknowledgment packets.

38. **IPV4**
   - IPv4 or Internet Protocol version 4, address is a 32-bit string of numbers separated by periods. It uniquely identifies a network interface in a device.IPv4 is the first non-experimental Internet Protocol.

39. **IPV6**
   - IPv6 is the latest version of the Internet Protocol, which identifies devices across the internet so they can be located. Every device that uses the internet is identified through its own IP address in order for internet communication to work.

40. **Dual Stacking**
   - Dual stack means that devices are able to run IPv4 and IPv6 in parallel. It allows hosts to simultaneously reach IPv4 and IPv6 content, so it offers a very flexible coexistence strategy.

41. **Tunneling**
   - Tunnelling is a protocol for transferring data securely from one network to another. Using a method known as encapsulation, Tunnelling allows private network communications to be sent across a public network, such as the Internet. Encapsulation enables data packets to appear general to a public network when they are private data packets, allowing them to pass unnoticed.

42. **Switches**
   - A network switch forwards data packets between devices. Switches send packets directly to devices, rather than sending them to networks like a router does. Switches can be hardware devices that manage physical networks, as well as software-based virtual devices.

43. **Bit**
   - A bit (binary digit) is the smallest unit of data that a computer can process and store. A bit is always in one of two physical states, similar to an on/off light switch. The state is represented by a single binary value, usually a 0 or 1. However, the state might also be represented by yes/no, on/off or true/false. Bits are stored in memory through the use of capacitors that hold electrical charges. The charge determines the state of each bit, which, in turn, determines the bit's value.

44. **Frames**
   - A frame is a unit of data. A frame works to help identify data packets used in networking and telecommunications structures. Frames also help to determine how data receivers interpret a stream of data from a source.

45. **Segment**
   - A process is divided into Segments. The chunks that a program is divided into which are not necessarily all of the same sizes are called segments. Segmentation gives user's view of the process which paging does not give. Here the user's view is mapped to physical memory.

46. **Ping**
   - Ping (Packet Internet Groper) is a method for determining communication latency between two networks. Simply put, ping is a method of determining latency or the amount of time it takes for data to travel between two devices or across a network. As communication latency decreases, communication effectiveness improves.

47. **Simple Mail Transfer Protocol**
   - The Simple Mail Transfer Protocol (SMTP) is a technical standard for transmitting electronic mail (email) over a network. Like other networking protocols, SMTP allows computers and servers to exchange data regardless of their underlying hardware or software. Just as the use of a standardized form of addressing an envelope allows the postal service to operate, SMTP standardizes the way email travels from sender to recipient, making widespread email delivery possible.

48. **File Transfer Protocol**
   - FTP (File Transfer Protocol) is a network protocol for transmitting files between computers over Transmission Control Protocol/Internet Protocol (TCP/IP) connections. Within the TCP/IP suite, FTP is considered an application layer protocol. In an FTP transaction, the end user's computer is typically called the local host. The second computer involved in FTP is a remote host, which is usually a server. Both computers need to be connected via a network and configured properly to transfer files via FTP.

49. **Address Resolution Protocol**
   - Address Resolution Protocol (ARP) is a procedure for mapping a dynamic IP address to a permanent physical machine address in a local area network (LAN). The physical machine address is also known as a media access control (MAC) address. The job of ARP is essentially to translate 32-bit addresses to 48-bit addresses and vice versa. This is necessary because IP addresses in IP version 4 (IPv4) are 32 bits, but MAC addresses are 48 bits.

50. **Internet Control Message Protocol**
   - The Internet Control Message Protocol (ICMP) is a network layer protocol used by network devices to diagnose network communication issues. ICMP is mainly used to determine whether or not data is reaching its intended destination in a timely manner. Commonly, the ICMP protocol is used on network devices, such as routers. ICMP is crucial for error reporting and testing, but it can also be used in distributed denial-of- service (DDoS) attacks.