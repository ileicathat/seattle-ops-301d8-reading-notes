Reading
Layers of OSI Model

1. What does “OSI” stand for?
> Open Systems Interconnection
2. List the 7 layers of the OSI model and what each one is responsible for.
> Layer 1- Physical Layer
The lowest layer of the OSI reference model is the physical layer. It is responsible for the actual physical connection between the devices. The physical layer contains information in the form of bits. It is responsible for transmitting individual bits from one node to the next. When receiving data, this layer will get the signal received and convert it into 0s and 1s and send them to the Data Link layer, which will put the frame back together.  

>Layer 2- Data Link Layer (DLL)
The data link layer is responsible for the node-to-node delivery of the message. The main function of this layer is to make sure data transfer is error-free from one node to another, over the physical layer. When a packet arrives in a network, it is the responsibility of the DLL to transmit it to the Host using its MAC address. 
The Data Link Layer is divided into two sublayers:  

Logical Link Control (LLC)
Media Access Control (MAC)
The packet received from the Network layer is further divided into frames depending on the frame size of the NIC(Network Interface Card). DLL also encapsulates Sender and Receiver’s MAC address in the header. 

The Receiver’s MAC address is obtained by placing an ARP(Address Resolution Protocol) request onto the wire asking “Who has that IP address?” and the destination host will reply with its MAC address.  

> Layer 3- Network Layer
The network layer works for the transmission of data from one host to the other located in different networks. It also takes care of packet routing i.e. selection of the shortest path to transmit the packet, from the number of routes available. The sender & receiver’s IP addresses are placed in the header by the network layer. 

The Functions of the Network Layer 
Routing: The network layer protocols determine which route is suitable from source to destination. This function of the network layer is known as routing.
Logical Addressing: To identify each device on Internetwork uniquely, the network layer defines an addressing scheme. The sender & receiver’s IP addresses are placed in the header by the network layer. Such an address distinguishes each device uniquely and universally.
Note: 1. Segment in the Network layer is referred to as Packet. 

          2. Network layer is implemented by networking devices such as routers. 

> Layer 4- Transport Layer
The transport layer provides services to the application layer and takes services from the network layer. The data in the transport layer is referred to as Segments. It is responsible for the End to End Delivery of the complete message. The transport layer also provides the acknowledgment of the successful data transmission and re-transmits the data if an error is found.

At the sender’s side: The transport layer receives the formatted data from the upper layers, performs Segmentation, and also implements Flow & Error control to ensure proper data transmission. It also adds Source and Destination port numbers in its header and forwards the segmented data to the Network Layer. 

Note: The sender needs to know the port number associated with the receiver’s application. 

Generally, this destination port number is configured, either by default or manually. For example, when a web application requests a web server, it typically uses port number 80, because this is the default port assigned to web applications. Many applications have default ports assigned. 

At the receiver’s side: Transport Layer reads the port number from its header and forwards the Data which it has received to the respective application. It also performs sequencing and reassembling of the segmented data. 

> Layer 5- Session Layer
This layer is responsible for the establishment of connection, maintenance of sessions, and authentication, and also ensures security.

> Layer 6- Presentation Layer
The presentation layer is also called the Translation layer. The data from the application layer is extracted here and manipulated as per the required format to transmit over the network. 

> Layer 7- Application Layer
At the very top of the OSI Reference Model stack of layers, we find the Application layer which is implemented by the network applications. These applications produce the data, which has to be transferred over the network. This layer also serves as a window for the application services to access the network and for displaying the received information to the user. 

3. Distinguish which layers are the “hardware layers”, and which layers are the “software layers”. What does that even mean?
> 5,6,7 are Software layers dealing primarily with information manipulation using programs

> 1,2,3,4 are hardware layers dealing with the transport of infomation over physical hardware and gateways

4. How can the OSI model be used in troubleshooting?

>Using the OSI we can split the network issues among these seven layers and can systematically troubleshoot a network. In any network, most of the problems occur at the physical, data-link, and network layers.

5. What Is Wireshark and How Is It Used?

Feel free to stop at “How to Use Wireshark”

6. What is Wireshark?
>A network packet capture tool. Wireshark will help you capture network packets and display them at a granular level. Once these packets are broken down, you can use them for real-time or offline analysis. This tool lets you put your network traffic under a microscope, and then filter and drill down into it, zooming in on the root cause of problems, assisting with network analysis and ultimately network security. 
7. What is a packet?
>In networking, a packet is a small segment of a larger message. Data sent over computer networks*, such as the Internet, is divided into packets. These packets are then recombined by the computer or device that receives them.

8. What 3 high-level things does Wireshark accomplish? How could these be used for nefarious purposes? For benevolent purposes?

>Packet Capture: Wireshark listens to a network connection in real time and then grabs entire streams of traffic – quite possibly tens of thousands of packets at a time.

>Filtering: Wireshark is capable of slicing and dicing all of this random live data using filters. By applying a filter, you can obtain just the information you need to see.

>Visualization: Wireshark, like any good packet sniffer, allows you to dive right into the very middle of a network packet. It also allows you to visualize entire conversations and network streams.

>If not used responsibly, it could be used to glean unauthorized information about a system or its users to compromise systems.

>Used responsibly, It can assist in identifying where network problems or security weaknesses may exist. 
