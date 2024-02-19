# Learning Objectives

- [OSI Model](#osi_model)
  -- What it is
  -- How many layers it has
  -- How it is organized
- [What is a LAN](#what_is_a_lan)
  -- Typical usage
  -- Typical geographical size
- [What is a WAN](#what_is_a_wan)
  -- Typical usage
  -- Typical geographical size
- [What is the Internet](#what_is_the_internet)
  -- What is an IP address
  -- What are the 2 types of IP address
  -- What is localhost
  -- What is a subnet
  -- Why IPv6 was created
- [TCP/UDP](#tcp_/_udp)
  -- What are the 2 mainly used data transfer protocols for IP (transfer level on the OSI schema)
  -- What is the main difference between TCP and UDP
  -- What is a port
  -- Memorize SSH, HTTP and HTTPS port numbers
  -- What tool/protocol is often used to check if a device is connected to a network

## exstra

- [ How to get my IP address](#how_to_get_my_ip_address)
- [ What is Mac address](#how_to_get_my_ip_address)

## 1, OSI Model

## What it is

from the International Organization for Standardization (ISO)
The OSI (Open Systems Interconnection) model is (from the International Organization for Standardization (ISO)) a conceptual framework that standardizes the functions of a communication or a network system into seven abstraction layers. Each layer serves a specific purpose and interacts with the adjacent layers, providing a systematic approach to understanding and designing network communication. The OSI model does not prescribe specific protocols but rather defines the tasks and functions each layer should perform. It enables interoperability between different network technologies and ensures that diverse systems can communicate seamlessly.

## How many layers it has

Seven

## How it is organized

<img src='https://msp.c.yimg.jp/images/v2/FUTi93tXq405grZVGgDqG-wR0ufwf4niEUhx_EbYBMiZI5JjPyEJWXqQnQtKM2cH5h3QwLRkno0QQuHJtKzMGiZEzckwNguskytMkemt2ZUKXYbOWjjB3LbAMv4-77T9lwk6jptChiJK5TKbZ6yKv2hOPlvbjxAe-g_GQ_t4p8zViKCf4P4NuEzCvIR40XkiD_nsWftuFF_fAP17pbTI2H9WqJkp9OCUVAIgpOsZKMXMZQhe6y-EXrWv_Bt9ZwnSvpgc3Jw6pE85-xMpC5Ijd2p9HCsNMeZA7-j3z2qoT0k=/Network-Components-8-min-1024x576.png?errorImage=false'>

### Physical Layer (Layer 1)

Deals with the physical connection between devices. It defines hardware specifications such as cables, connectors, and electrical signals.

- Data Format:
  -- Raw bits.
- Sender Side:
  -- Converts data into bits.
  -- Transmits raw bits over the physical medium.
- Receiver Side:
  -- Receives raw bits from the physical medium

### Data Link Layer (Layer 2)

Responsible for the reliable transmission of data frames between devices on the same network. It includes sublayers for addressing (MAC addresses) and error detection.¥

- Data Format:
  -- Frames.
- Sender Side:
  -- Frames the data by adding headers and trailers.
  -- Performs error detection and correction.
  -- Transmits frames.
- Receiver Side:
  -- Receives frames.
  -- Performs error detection and correction.
  -- Strips headers and trailers to extract data.

### Network Layer (Layer 3)

Focuses on logical addressing and routing. It determines the best path for data to travel from the source to the destination across multiple networks.

- Data Format:
  -- Packets.
- Sender Side:
  -- Adds logical addressing to create packets.
  -- Determines the best path for packet transmission.
- Receiver Side:
  -- Receives packets.
  -- Routes packets to the correct destination.

### Transport Layer (Layer 4)

Ensures end-to-end communication by managing error detection, correction, and data flow control. It divides large messages into smaller segments and reassembles them at the destination.

- Data Format:
  -- Segments.
- Sender Side:
  -- Divides data into segments.
  -- Adds segment headers.
  -- Manages end-to-end communication, error detection, and flow control.
- Receiver Side:
  -- Receives segments.
  -- Performs error detection and flow control.
  -- Reassembles segments into data.

### Session Layer (Layer 5)

Establishes, manages, and terminates communication sessions between applications. It ensures that data exchange occurs in an organized and synchronized manner.

- Data Format:
  -- Data.
- Sender Side:
  -- Establishes, maintains, and terminates sessions.
  -- Synchronizes data exchange.

- Receiver Side:
  -- Receives and manages sessions.
  -- Synchronizes data exchange.

### Presentation Layer (Layer 6)

Deals with data translation, encryption, and compression. It transforms data into a format that can be understood by the application layer.

- Data Format:
  -- Data.
- Sender Side:
  -- Translates, encrypts, or compresses data.
- Receiver Side:
  -- Translates, decrypts, or decompresses data.

### Application Layer (Layer 7)

The topmost layer interacts directly with end-user applications. It provides network services such as file transfers, email, and remote login, allowing software to communicate over a network.

- Data Format:
  -- Data.

- Sender Side:
  -- Provides network services to applications.
  -- Interacts with end-user applications.

- Receiver Side:
  -- Provides network services to applications.
  -- Interacts with end-user applications.

## What is a LAN

A LAN, or Local Area Network, is a network of interconnected computers, devices, and resources within a limited geographic area, such as a home, office, or campus. LANs are designed to facilitate communication and resource sharing among devices in close proximity to each other.

### Typical usage

There are numerous use cases for Local Area Networks (LANs), as they are commonly employed in various settings to facilitate communication, resource sharing, and collaboration within a localized geographic area.

- Office Networking:
  -- Scenario: In an office environment, LANs connect computers, printers, servers, and other devices to enable seamless communication and resource sharing.
  -- Use Case: Employees can share files, access shared printers, and collaborate on projects through networked applications. LANs improve efficiency and promote collaboration within the office.

- Home Networking:
  -- Scenario: In a home setting, LANs connect devices such as computers, laptops, smartphones, smart TVs, and printers.
  -- Use Case: Family members can share files, stream media, and access shared printers or networked storage. Home LANs also enable internet connectivity for multiple devices through a single connection.

- Educational Institutions:
  -- Scenario: Schools, colleges, and universities deploy LANs to connect computers, servers, and educational resources within a campus.
  -- Use Case: Students and teachers can access shared educational materials, collaborate on projects, and use networked resources, fostering a more interactive and connected learning environment.

- Small Business Networking:
  -- Scenario: Small businesses utilize LANs to connect workstations, servers, and networked devices.
  -- Use Case: Employees can collaborate on projects, access shared databases, and share resources like printers. LANs contribute to the overall productivity and efficiency of small businesses.

### Typical geographical size

The typical geographical size of a Local Area Network (LAN) can vary,
but it is generally limited to a relatively small and localized aree, such as schools, hospitals and offices

## What is a WAN

A WAN, or Wide Area Network, is a type of computer network that extends over a large geographical area, connecting multiple LANs (Local Area Networks) and other network devices across cities, countries, or even continents. WANs are designed to facilitate long-distance communication and data exchange between different locations.

- Scope: WANs cover a broad geographical area, connecting LANs and other network devices across extensive distances. They can span regional, national, or global scales.

### Typical usage

- Interconnecting Branch Offices:
  -- Scenario:
  A company with multiple branch offices or regional locations needs to establish a network that connects all offices.
  -- Use Case:
  WANs allow seamless communication and resource sharing between branch offices, enabling centralized management, data access, and collaboration.

- Global Corporate Networks:
  -- Scenario:
  Multinational corporations with offices or subsidiaries in different countries require a network infrastructure that spans the globe.
  -- Use Case:
  WANs support global communication, data transfer, and collaboration among employees, ensuring that the organization operates cohesively across international borders.

- Remote Access for Employees:
  -- Scenario:
  Organizations with employees working remotely or from home locations need to provide secure access to corporate resources.
  -- Use Case:
  WAN technologies, such as VPNs (Virtual Private Networks), enable secure connectivity for remote employees to access company databases, applications, and internal systems.

- Connecting Data Centers:
  -- Scenario:
  Companies with multiple data centers in different locations seek to establish reliable and high-speed connections between these facilities.
  -- Use Case:
  WANs support data replication, backup, and disaster recovery strategies by connecting geographically distributed data centers. This ensures redundancy and data availability.

- Global Collaboration and Communication:
  -- Scenario:
  Organizations that collaborate on projects or have distributed teams across different regions.
  -- Use Case:
  WANs facilitate real-time communication, video conferencing, and collaborative work environments for teams working across the globe.

### Typical geographical size

The typical geographical size of a Wide Area Network (WAN) can vary significantly based on the specific requirements of the organization or the nature of the network. Unlike Local Area Networks (LANs), which are limited to a relatively small geographic area, WANs cover larger distances, connecting multiple LANs and other network devices.

- Regional WANs:
  -- Size:
  Covers a region, such as a city, state, or a specific geographic area.
  -- Example:
  A company with multiple offices within a city or state might establish a regional WAN to interconnect these locations.

- National WANs:
  -- Size: Spans an entire country or a large portion of a country.
  -- Example: A nationwide corporation with offices and branches in different cities or states might deploy a national WAN to connect these locations.

- Global WANs:
  -- Size: Extends internationally, connecting locations across different countries or continents.
  -- Example: Multinational corporations with offices, subsidiaries, or data centers worldwide use global WANs to facilitate communication and collaboration on a global scale.

- Intercontinental WANs:
  -- Size: Spans multiple continents, connecting locations across the globe.
  -- Example: Large enterprises, research institutions, or organizations with a global presence may require intercontinental WANs to link their operations and resources across continents.

- Internet as a WAN:
  -- Size: The entire internet serves as a WAN.
  -- Example: The internet itself is a global WAN that connects networks, servers, and devices worldwide. Organizations can leverage the internet for WAN connectivity through VPNs or direct connections.

## What is the Internet?

The Internet is a global network of interconnected computer networks that use standardized communication protocols to link devices and facilitate the exchange of information.

### What is an IP address

An IP address, or Internet Protocol address, is a numerical label assigned to each device connected to a computer network that uses the Internet Protocol for communication. IP addresses serve two main purposes in networking: host or network interface identification and location addressing. They play a crucial role in the routing of data packets across networks.

### What are the 2 types of IP address

There are two versions of IP addresses commonly used today:

- IPv4 (Internet Protocol version 4):

Consists of 32 bits, represented as four sets of octets (each octet being 8 bits) separated by dots.
Example: 192.168.0.1

- IPv6 (Internet Protocol version 6):

Uses a longer address space, represented as 128 bits, allowing for a vastly larger number of unique addresses compared to IPv4.
Example: 2001:0db8:85a3:0000:0000:8a2e:0370:7334

### What is localhost

"Localhost" refers to the loopback network address, typically designated as 127.0.0.1 in IPv4 or ::1 in IPv6. It is used to access the network services that are running on the host via the network interface itself. In simpler terms, localhost points to the current device or machine that a user is working on.

### What is a subnet

A subnet, short for "subnetwork," is a logical division of an IP network into smaller, more manageable segments. Subnetting is a technique used to create subnetworks within a larger network, allowing for efficient utilization of IP addresses and providing benefits such as improved network performance, security, and organization. Subnetting is commonly employed in IPv4 networks.

Subnetting involves dividing a larger IP network into smaller, more manageable pieces or subnetworks, each with its own unique range of IP addresses. These subnets are isolated from each other logically, creating separate segments within the overall network. Each subnet functions as an independent network within the larger network infrastructure.

### Why IPv6 was created

IPv6, or Internet Protocol version 6, was created to address the limitations of its predecessor, IPv4 (Internet Protocol version 4), and to overcome the challenges posed by the exhaustion of IPv4 address space.

## TCP/UDP

The two main data transfer protocols at the transport layer (Layer 4) of the OSI model for IP (Internet Protocol) are TCP and UDP

### Transmission Control Protocol (TCP):

- Characteristics:
  -- Connection-oriented:
  Establishes a reliable, two-way communication channel between devices before data transfer.
  -- Flow control:
  Manages the rate of data exchange to prevent congestion and ensure reliable delivery.
  -- Error detection and correction:
  Implements mechanisms to detect and recover from errors in data transmission.
  -- Sequencing:
  Orders and reorders data packets to ensure correct delivery.
  -- Use Cases:
  Reliable data transfer, such as file transfers and web page loading.
  Applications requiring guaranteed delivery and accurate sequencing of data.
  -- Examples:
  - HTTP (Hypertext Transfer Protocol) for web browsing.
  - FTP (File Transfer Protocol) for file transfers.
  - SMTP (Simple Mail Transfer Protocol) for email transmission.

### User Datagram Protocol (UDP):

- Characteristics:
  -- Connectionless:
  Does not establish a connection before sending data, providing a simpler, faster communication model.
  -- Unreliable:
  Does not guarantee delivery, and there is no mechanism for error recovery.
  -- Low overhead:
  Minimal protocol overhead compared to TCP, making it suitable for real-time applications.
  -- Use Cases:
  Real-time applications where low latency is critical.
  Streaming media, online gaming, VoIP (Voice over Internet Protocol).
  -- Examples:
  - DNS (Domain Name System) for translating domain names to IP addresses.
  - DHCP (Dynamic Host Configuration Protocol) for IP address assignment.
  - SNMP (Simple Network Management Protocol) for network management.

### What is the main difference between TCP and UDP

The main differences between TCP (Transmission Control Protocol) and UDP (User Datagram Protocol) lie in their connection-oriented nature, reliability, data transfer mechanism, and overhead.

- Connection-Oriented vs. Connectionless:
  -- TCP:
  Connection-oriented protocol. Before data transfer, a reliable connection is established between the sender and receiver. This connection ensures data integrity, sequencing, and error recovery.
  -- UDP:
  Connectionless protocol. It does not establish a connection before sending data. Each UDP packet is sent independently, and there is no inherent concept of a connection.

- Reliability:
  -- TCP: Reliable protocol. It ensures that data is delivered accurately and in the correct order. If packets are lost or corrupted during transmission, TCP retransmits them to guarantee delivery.
  -- UDP: Unreliable protocol. It does not provide mechanisms for error detection, correction, or retransmission. Packets may be lost, duplicated, or delivered out of order.

- Flow Control:
  -- TCP: Implements flow control mechanisms to manage the rate of data exchange between sender and receiver. It prevents congestion and ensures that the sender does not overwhelm the receiver with data.
  -- UDP: No inherent flow control. UDP relies on the application layer to handle flow control if needed.

- Order of Delivery:
  -- TCP: Ensures the correct sequencing of data packets. If packets arrive out of order, TCP reorders them before delivering the data to the application layer.
  -- UDP: Does not guarantee the order of delivery. Packets may arrive out of order, and it is the responsibility of the application layer to manage sequencing if required.

- Overhead:
  -- TCP: Higher overhead due to the need for connection establishment, flow control, and reliability mechanisms. This results in a more complex protocol.
  -- UDP: Lower overhead compared to TCP. Its connectionless nature and lack of elaborate mechanisms make it a simpler and faster protocol.

- Usage Scenarios:
  -- TCP: Suitable for applications where data integrity and sequencing are crucial, such as file transfers, web browsing, and email.
  -- UDP: Ideal for real-time applications with low-latency requirements, such as streaming media, online gaming, and VoIP (Voice over Internet Protocol).

## What is a port

A port is a communication endpoint or interface through which processes on different devices can exchange data. Ports are essential for enabling communication between applications or services running on a computer or networked devices. Ports are associated with specific protocols and are identified by numerical values known as port numbers.

- Port Numbers:
  -- A port number is a 16-bit unsigned integer, which means it can range from 0 to 65535.
- Ports are categorized into three ranges:
  -- Well-known ports (0-1023): Reserved for standard services and protocols.
  -- Registered ports (1024-49151): Assigned by the Internet Assigned Numbers Authority (IANA) for specific applications.
  -- Dynamic or private ports (49152-65535): Available for dynamic assignment by applications and services.

- Transport Layer:
- Ports operate at the transport layer (Layer 4) of the OSI model. They work in conjunction with IP addresses to facilitate communication between devices on a network.
- Protocol Multiplexing:
  -- The combination of an IP address and a port number allows multiple services or applications to run on the same device without conflict. This is known as protocol multiplexing.
  -- Well-Known Ports:

  - Port 80: Used for HTTP (Hypertext Transfer Protocol).
  - Port 443: Used for HTTPS (Hypertext Transfer Protocol Secure).
  - Port 21: Used for FTP (File Transfer Protocol).
  - Port 25: Used for SMTP (Simple Mail Transfer Protocol).

- Dynamic Ports:
  Many applications and services use dynamic or ephemeral ports (those above 49151) for communication. These ports are assigned by the operating system when a connection is established and are released when the connection is terminated.

- Socket:
  A combination of IP address and port number is referred to as a socket. Sockets uniquely identify communication endpoints in a network.

- Local and Remote Ports:
  In a communication session, there is a local port (used by the sender) and a remote port (used by the receiver). Together, they define the source and destination of the data transfer.

- Firewall Configuration:
  Firewalls use port numbers to control and filter network traffic. Administrators can configure firewalls to allow or block traffic based on specific port numbers.

## Memorize SSH, HTTP and HTTPS port numbers

SSH (Secure Shell):

Port Number: 22
HTTP (Hypertext Transfer Protocol):

Port Number: 80
HTTPS (HTTP Secure):

Port Number: 443

## What tool/protocol is often used to check if a device is connected to a network

One common tool used to check if a device is connected to a network is the "Ping" utility, which operates based on the Internet Control Message Protocol (ICMP). ICMP is a network layer protocol that allows devices to send error messages and other operational information about network conditions.

### Ping (Packet Internet Groper):

- Ping is a command-line utility available on most operating systems (such as Windows, macOS, and Linux/Unix).
  It sends ICMP Echo Request messages to a specified IP address or hostname.

### ICMP Echo Request and Reply:

When a device receives an ICMP Echo Request, it responds with an ICMP Echo Reply if it is reachable and connected to the network.
If the device is not reachable or connected, no reply is received.

```bash
ping 192.168.1.1
```

## How to get my IP address?

For mac

```bash
ipconfig getifaddr en1
```

## What is Mac address

A MAC address (Media Access Control address) is a unique identifier assigned to network interfaces for communications on a physical network. It is a hardware address and is associated with the Data Link Layer (Layer 2) of the OSI model. MAC addresses are used to uniquely identify devices within a local network.

### Uniqueness:

- Each MAC address is globally unique. Manufacturers are assigned blocks of MAC addresses, and they are responsible for ensuring that each network interface they produce has a unique MAC address.

### Length and Format:

- A MAC address is 48 bits long, typically represented as six groups of two hexadecimal digits (0-9, A-F), separated by colons or hyphens. For example, 01:23:45:67:89:ab.

### Addressing at the Data Link Layer:

- MAC addresses operate at the Data Link Layer (Layer 2) of the OSI model. They are used for communication within the same local network and are not routed across different subnets.

### Role in Ethernet Networks:

- In Ethernet networks, MAC addresses are crucial for the delivery of frames. Each Ethernet frame includes the source and destination MAC addresses in the header.

### Addressing in Network Devices:

Network devices, such as network interface cards (NICs) in computers, routers, switches, and other devices, have a unique MAC address burned into their hardware during manufacturing.

### OUI (Organizationally Unique Identifier):

The first 24 bits of a MAC address represent the OUI, which is assigned to the manufacturer of the network interface card. The remaining 24 bits are typically unique to each device produced by that manufacturer.

### Dynamic and Static Assignment:

MAC addresses can be assigned dynamically (e.g., through DHCP) or statically (manually configured) depending on the network configuration.

### Use in Address Resolution Protocol (ARP):

MAC addresses are involved in the Address Resolution Protocol (ARP) process, where devices map IP addresses to MAC addresses within a local network.

### Role in Switching:

MAC addresses are used by network switches to forward frames to the correct port. Switches build and maintain MAC address tables to efficiently forward frames within the local network.
