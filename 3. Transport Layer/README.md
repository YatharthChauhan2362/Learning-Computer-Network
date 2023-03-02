# **WELCOME TO LEARN COMPUTER NETWORK**

    AUTHOR:         Yatharth Chauhan  (Github: YatharthChauhan2362)
    SUBJECT:        Computer Network
    REPOSITORY:     Learning-Computer-Network

# CHAPTER-3: Transport Layer

## Introduction

The Transport Layer is the fourth layer of the OSI (Open Systems Interconnection) and TCP/IP (Transmission Control Protocol/Internet Protocol) network models. Its primary function is to provide end-to-end data transport services between applications running on different hosts or devices.

The Transport Layer is responsible for ensuring reliable data transfer between source and destination hosts by establishing connections, managing data segmentation and reassembly, and performing error detection and correction. The most common protocols at this layer are TCP (Transmission Control Protocol) and UDP (User Datagram Protocol).

TCP provides reliable, connection-oriented data transfer services by establishing a virtual circuit between the source and destination hosts before transferring data. It breaks data into segments, adds sequencing and error checking information, and reassembles them at the receiver end. TCP provides flow control and congestion control mechanisms to ensure that data is transmitted at an optimal rate and to avoid network congestion.

UDP, on the other hand, is a connectionless, unreliable protocol that provides best-effort data transfer services. It does not establish a connection before transferring data and does not perform error correction or flow control. UDP is used for applications that require low-latency and high-throughput, such as real-time multimedia streaming, online gaming, and voice-over-IP (VoIP).

In summary, the Transport Layer is responsible for providing end-to-end data transport services, including reliability, error detection and correction, flow control, and congestion control. TCP and UDP are the most commonly used protocols at this layer, with TCP providing reliable, connection-oriented data transfer services, and UDP providing best-effort, connectionless data transfer services.

## Transport-Layer Services

Transport Layer Services are an essential component of the Internet Protocol (IP) suite. The Transport layer is responsible for delivering data reliably and efficiently between applications running on different hosts connected over a network. Some of the key services provided by the Transport Layer include:

1. Connection-oriented communication:

- The Transport Layer provides connection-oriented communication through the use of protocols like Transmission Control Protocol (TCP). Connection-oriented communication ensures that the data is delivered reliably and in order.

2. Connectionless communication:

- The Transport Layer also provides connectionless communication through the use of User Datagram Protocol (UDP). Connectionless communication is faster and more efficient than connection-oriented communication but does not guarantee reliable data delivery.

3. Multiplexing:

- The Transport Layer allows multiple applications to use the same network connection simultaneously. This is achieved through multiplexing, which involves assigning unique identifiers (port numbers) to each application.

4. Flow control:

- The Transport Layer is responsible for managing the flow of data between hosts to ensure that data is not lost or delayed. Flow control helps prevent congestion in the network by regulating the rate at which data is transmitted.

5. Error control:

- The Transport Layer provides error control to detect and recover from transmission errors that may occur during data transfer.

6. Segmentation and reassembly:

- The Transport Layer segments large amounts of data into smaller, manageable pieces, and reassembles them at the destination.

7. Quality of Service (QoS):

- The Transport Layer provides Quality of Service (QoS) by allowing applications to specify the level of service required for their data. QoS ensures that high-priority data is given preferential treatment over low-priority data.

## Multiplexing and Demultiplexing

Multiplexing and demultiplexing are two key concepts in computer networking that are used to transmit multiple signals over a single communication channel. Multiplexing is the process of combining multiple data streams into a single signal, while demultiplexing is the process of separating the single signal back into its original multiple data streams.

In networking, multiplexing is often used to combine multiple data streams from different sources into a single transmission medium, such as a cable or wireless channel. This can help increase the efficiency of network communication, as multiple data streams can be transmitted simultaneously over the same channel.

There are several different types of multiplexing techniques used in networking, including:

1. Time Division Multiplexing (TDM): This technique assigns specific time slots to different data streams. Each stream is given a small amount of time to transmit its data before the next stream is allowed to transmit.

2. Frequency Division Multiplexing (FDM): This technique assigns different frequency ranges to different data streams. Each stream is assigned a specific frequency range to transmit its data.

3. Code Division Multiplexing (CDM): This technique assigns different codes to different data streams. Each stream uses a different code to transmit its data, allowing multiple streams to be transmitted simultaneously.

Demultiplexing is the process of separating the multiplexed signal back into its original data streams. Demultiplexing is typically performed by the receiving device, which separates the incoming signal into its constituent data streams based on the multiplexing technique used.

Overall, multiplexing and demultiplexing are key techniques used in networking to increase the efficiency of communication over a single channel.

## Connectionless Transport: UDP & Building Blocks of UDP

Connectionless transport is a type of data transport mechanism used in computer networking, where data is transmitted between two network entities without the establishment of a dedicated connection. The most common protocol used for connectionless transport is the User Datagram Protocol (UDP).

UDP is a lightweight protocol that is designed for fast and efficient data transmission. Unlike connection-oriented protocols such as TCP, UDP does not establish a dedicated connection before data transmission, and there is no guarantee that the data will be received by the recipient. However, the speed and simplicity of UDP make it an ideal protocol for applications that require real-time data transmission, such as video and audio streaming.

The building blocks of UDP include:

1. Source port: This is a 16-bit field that identifies the port number used by the sending application.

2. Destination port: This is a 16-bit field that identifies the port number used by the receiving application.

3. Length: This is a 16-bit field that specifies the length of the UDP header and data in bytes.

4. Checksum: This is a 16-bit field that provides error checking for the UDP datagram. The checksum is calculated by the sending host and verified by the receiving host.

5. Data: This is the payload of the UDP datagram, which contains the actual data being transmitted.

UDP is often used in conjunction with other protocols, such as the Internet Protocol (IP), to provide reliable data transmission over the internet. While UDP does not provide any guarantees for data delivery, it is a fast and efficient protocol that is well-suited for real-time applications where speed is more important than reliability.

## Principles of Reliable Data Transfer

Reliable data transfer refers to the delivery of data between two network devices with a high degree of accuracy and certainty. In networking, there are several principles that ensure reliable data transfer, including:

1. Acknowledgment:

- When a device receives a data packet, it sends an acknowledgment (ACK) to the sender to confirm receipt. If the sender does not receive an ACK, it assumes that the packet was lost and retransmits the packet.

2. Sequence Numbers:

- Each data packet is assigned a unique sequence number that identifies the order in which it was sent. The receiver uses these sequence numbers to ensure that packets are delivered in the correct order.

3. Retransmission:

- If a sender does not receive an ACK, it retransmits the packet. This process continues until the sender receives an ACK or until a predetermined number of retransmissions has occurred.

4. Timeout:

- A timeout mechanism is used to ensure that a sender does not wait indefinitely for an ACK. If an ACK is not received within a specified period, the sender assumes that the packet was lost and retransmits the packet.

5. Flow Control:

- Flow control mechanisms are used to ensure that a sender does not overwhelm a receiver with too much data. These mechanisms allow the receiver to control the rate at which data is sent.

6. Error Detection and Correction:

- Error detection and correction techniques are used to ensure that data is transmitted accurately. These techniques include checksums and cyclic redundancy checks (CRCs).

By adhering to these principles, network devices can ensure reliable data transfer, which is critical for the successful transmission of data across a network.

## Connection-Oriented Transport

Connection-oriented transport is a type of network communication protocol in which a dedicated and reliable end-to-end communication path is established before any data transmission occurs. This ensures that the communication is reliable and the data is transmitted in the correct order without any loss or duplication.

In connection-oriented transport, a session is first established between the two endpoints (e.g., two computers). This involves a three-way handshake process, where the two endpoints exchange control messages to establish the connection, negotiate parameters, and synchronize their sequence numbers.

Once the connection is established, data can be transmitted between the two endpoints. Each data packet is typically acknowledged by the receiver, and retransmission is performed in case of errors or timeouts. At the end of the session, a connection termination process is performed to release the resources and terminate the connection.

TCP (Transmission Control Protocol) is an example of a connection-oriented transport protocol commonly used in the Internet. It provides reliable, ordered, and error-checked delivery of data between applications running on hosts in IP networks. Other examples of connection-oriented protocols include ATM (Asynchronous Transfer Mode) and X.25.
