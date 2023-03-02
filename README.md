# Learning-Computer-Network
Let's Learn Together and Grow Together - Yatharth Chauhan

# Protocols

In networking, a protocol refers to a set of rules or standards that govern the way devices communicate with each other over a network. A protocol determines how data is transmitted, received, and processed over the network.

Protocols are essential for enabling communication between different devices and ensuring that the data is transmitted correctly and reliably. There are many different types of protocols used in networking, including:

1. Transmission Control Protocol/Internet Protocol (TCP/IP) 
- This is the most widely used protocol suite for communication on the internet.

2. User Datagram Protocol (UDP) 
- A lightweight protocol used for quick data transmission where reliability is not the primary concern.

3. Hypertext Transfer Protocol (HTTP) 
- A protocol used for transmitting web pages and other data over the internet.

4. Simple Mail Transfer Protocol (SMTP) 
- A protocol used for sending email messages over the internet.

5. File Transfer Protocol (FTP) 
- A protocol used for transferring files between computers over the internet.

Each protocol has its own specific set of rules and standards that devices must follow to ensure successful communication.

# Access Networks

Access networks, in networking, refer to the portion of a telecommunications network that connects subscribers or end-users to the core network or the internet.

There are different types of access networks, including:

1. Wired access networks 
- These networks use physical cables, such as copper or fiber optic cables, to connect end-users to the network. Examples of wired access networks include Digital Subscriber Line (DSL), cable modem, and Ethernet.

2. Wireless access networks 
- These networks use wireless signals, such as radio waves or microwave, to connect end-users to the network. Examples of wireless access networks include Wi-Fi, cellular networks, and satellite networks.

Access networks are essential for providing users with access to network services, such as the internet, voice, and video. They also play a crucial role in determining the quality of service that end-users receive, including factors such as bandwidth, latency, and reliability.

In summary, access networks are the final link between end-users and the telecommunications network or the internet. They are critical to providing access to network services and determining the quality of service that end-users receive.

# Physical media

Physical media in networking refers to the type of cables and wires that are used to transmit data between devices on a network. There are several types of physical media commonly used in networking:

1. Twisted Pair: 
- Twisted pair cables are the most commonly used type of cable in networking. They consist of pairs of copper wires twisted together to reduce interference and crosstalk.

2. Coaxial Cable: 
- Coaxial cable is a type of cable consisting of a central conductor surrounded by an insulating layer, a conductive shield, and a protective outer jacket. It is used in cable television and some networking applications.

3. Fiber Optic Cable: 
- Fiber optic cable uses thin strands of glass or plastic to transmit data over long distances. It offers very high bandwidth and is used in high-speed networking applications.

4. Wireless: 
- Wireless networking uses radio waves to transmit data between devices. It eliminates the need for physical cables but can be affected by interference from other devices.

The choice of physical media depends on factors such as the distance between devices, the speed of the network, and the level of interference present in the environment.

# Packet Switching & Circuit Switching

Packet switching and circuit switching are two different methods of transmitting data over a network.

Circuit Switching

- Circuit switching is an older technology that is used in traditional telephone networks. It works by creating a dedicated physical connection, or circuit, between two devices for the duration of the communication. The circuit is reserved exclusively for the two devices and cannot be used by anyone else. This means that the communication is uninterrupted, but it also means that the circuit remains occupied even when no data is being transmitted, leading to inefficient use of resources.

Packet switching
- Packet switching, on the other hand, is the method used in modern computer networks, including the internet. In packet switching, data is broken down into small packets and sent over the network individually. Each packet contains a portion of the data, as well as the address of its destination. The packets travel through the network separately and can take different paths to reach their destination. When they arrive at their destination, they are reassembled into the original message. Packet switching allows multiple devices to share the same network resources, which makes it more efficient than circuit switching.

In summary, circuit switching creates a dedicated physical connection between two devices for the duration of the communication, while packet switching breaks data down into small packets and sends them individually over the network, allowing multiple devices to share the same network resources. Packet switching is the method used in modern computer networks, while circuit switching is an older technology used in traditional telephone networks.


# Delay and Loss

Delay refers to the time it takes for data to travel from one point to another in a network. There are several types of delay that can occur in a network:

1. Transmission delay: The time it takes for a node to transmit data onto the network.

2. Propagation delay: The time it takes for data to travel from one end of a network to the other.

3. Processing delay: The time it takes for a node to process data before transmitting it onto the network.

4. Queuing delay: The time it takes for data to wait in a queue before it can be transmitted.

5. Network congestion delay: The time it takes for data to be delayed due to congestion in the network.

On the other hand, loss in networking refers to the situation where some of the transmitted data is not received at the destination. There are several reasons why data loss can occur in a network, including:

1. Network congestion: When the network is congested, packets may be dropped to alleviate the congestion.

2. Interference: Physical interference in the network can cause data loss.

3. Faulty equipment: Malfunctioning hardware can cause packets to be lost.

4. Errors in data transmission: Transmission errors can cause packets to be lost or corrupted.

Both delay and loss can impact the performance and reliability of a network, and therefore it is important to monitor and manage these issues in order to maintain a high-quality network.

# Throughput

Throughput is the amount of data that can be transmitted over a network in a given amount of time. In packet-switched networks, throughput is affected by several factors, including the size of the packets, the available bandwidth, and the number of packets being transmitted.

Packet-switched networks divide data into packets, which are sent individually across the network and reassembled at the destination. The size of the packets can affect the throughput of the network, as larger packets take longer to transmit than smaller packets. However, larger packets can be more efficient, as there is less overhead associated with transmitting a larger number of smaller packets.

Bandwidth is another factor that affects the throughput of packet-switched networks. Bandwidth refers to the amount of data that can be transmitted over the network in a given amount of time. A network with a high bandwidth can transmit more data in a given amount of time than a network with a lower bandwidth.

Finally, the number of packets being transmitted can also affect the throughput of a packet-switched network. As more packets are transmitted, the network may become congested, which can result in delays and packet loss. This can reduce the overall throughput of the network.

To optimize throughput in packet-switched networks, it is important to balance the size of the packets with the available bandwidth and to manage congestion to minimize delays and packet loss. Network administrators may use tools such as Quality of Service (QoS) to prioritize traffic and manage congestion in order to maximize network throughput.

# Queuing Delay

Queuing delay is a type of delay that can occur in packet-switched networks when packets are queued up in a buffer.

In packet-switched networks, packets are transmitted in small units and are routed through the network from source to destination. As these packets arrive at intermediate network devices such as routers, they are stored temporarily in a buffer before being forwarded to the next device.

If the buffer is full, incoming packets will have to wait in a queue until space becomes available. The time that a packet spends waiting in this queue is known as queuing delay.

Queuing delay can vary depending on the length of the queue, the number of packets in the queue, and the rate at which packets are arriving. When the queue is empty, the queuing delay is zero. However, as the number of packets in the queue increases, so does the queuing delay.

Queuing delay can have a significant impact on network performance, especially in networks that experience high traffic or congestion. To minimize queuing delay, network administrators can implement techniques such as traffic shaping, prioritization, and packet dropping policies.

