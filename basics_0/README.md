# Networking basics #0

This repository serves as a comprehensive guide to net working basics.
This collection has been crafted to provide an immersive and hands-on learning experience, and to deepen their understanding of networking concepts.

## Table of Contents

- [Learning Objectives](#learning-objectives)
- [Requirements](#requirements)
- [Practice Exercises](#practice-exercises)

## Learning Objectives

This project is based on the learning objectives - see the [LEARNING_OBJECTIVES](https://github.com/Goaty-yagi/holbertonschool-network/blob/main/basics_0/LEARNING_OBJECTIVES.md) file for details.

## Requirements

- Allowed editors: vi, vim, emacs
- All your Bash script files will be interpreted on Ubuntu 20.04 LTS
- All your files should end with a new line
- A README.md file, at the root of the folder of the project, is mandatory
- All your Bash script files must be executable
- Your Bash script must pass shellcheck without any error
- The first line of all your Bash scripts should be exactly #!/usr/bin/env bash
- The second line of all your Bash scripts should be a comment explaining what is the script doing

## Practice Exercises

### 0. OSI model

**File:** [0-OSI_model](https://github.com/Goaty-yagi/holbertonschool-network/blob/main/basics_0/0-OSI_model)<br>
**Description:** <br>
What is the OSI model?

- 1, Set of specifications that network hardware manufacturers must respect
- 2, The OSI model is a conceptual model that characterizes the communication functions of a telecommunication system without regard to their underlying internal structure and technology
- 3, The OSI model is a model that characterizes the communication functions of a telecommunication system with a strong regard for their underlying internal structure and technology

How is the OSI model organized?

- 1, Alphabetically
- 2, From the lowest to the highest level
- 3, Randomly

### 1. Types of network

**File:** [1-types_of_network](https://github.com/Goaty-yagi/holbertonschool-network/blob/main/basics_0/1-types_of_network)<br>
**Description:** <br>
What type of network a computer in local is connected to?

- 1, Internet
- 2, WAN
- 3, LAN

What type of network could connect an office in one building to another office in a building a few streets away?

- 1, Internet
- 2, WAN
- 3, LAN

What network do you use when you browse www.google.com from your smartphone (not connected to the Wifi)?

- 1, Internet
- 2, WAN
- 3, LAN

### 2. MAC and IP address

**File:** [2-MAC_and_IP_address](https://github.com/Goaty-yagi/holbertonschool-network/blob/main/basics_0/2-MAC_and_IP_address)<br>
**Description:** <br>
What is a MAC address?

- 1, The name of a network interface
- 2, The unique identifier of a network interface
- 3, A network interface

What is an IP address?

- 1, Is to devices connected to a network what postal address is to houses
- 2, The unique identifier of a network interface
- 3, Is a number that network devices use to connect to networks

### 3. UDP and TCP

**File:** [3-UDP_and_TCP](https://github.com/Goaty-yagi/holbertonschool-network/blob/main/basics_0/3-UDP_and_TCP)<br>
**Description:** <br>

<img src='https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2020/9/3d92e3c4a470f8ecf4c73db511fcbbadaa002e1c.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20240219%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20240219T002511Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=e100c747cf7c983ad2d264137972b24a66690d43330291a9bac2dd94ff756503'>

Let’s fill the empty parts in the drawing above.

Questions:

- Which statement is correct for the TCP box:
  -- It is a protocol that is transferring data in a slow way but surely
  -- It is a protocol that is transferring data in a fast way and might loss data along in the process
- Which statement is correct for the UDP box:
  -- It is a protocol that is transferring data in a slow way but surely
  -- It is a protocol that is transferring data in a fast way and might loss data along in the process
- Which statement is correct for the TCP worker:
  -- Have you received boxes x, y, z?
  -- May I increase the rate at which I am sending you boxes?

### 4. TCP and UDP ports

**File:** [4-TCP_and_UDP_ports](https://github.com/Goaty-yagi/holbertonschool-network/blob/main/basics_0/4-TCP_and_UDP_ports)<br>
**Description:** <br>

Write a Bash script that displays listening ports:

That only shows listening sockets
That shows the PID and name of the program to which each socket belongs


### 5. Is the host on the network

**File:** [5-is_the_host_on_the_network](https://github.com/Goaty-yagi/holbertonschool-network/blob/main/basics_0/5-is_the_host_on_the_network)<br>
**Description:** <br>
Write a Bash script that pings an IP address passed as an argument.
**Requirement:** <br>
- Accepts a string as an argument
- Displays Usage: 5-is_the_host_on_the_network {IP_ADDRESS} if no argument passed
- Ping the IP 5 times
