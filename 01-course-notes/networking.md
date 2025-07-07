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
     
     
    













