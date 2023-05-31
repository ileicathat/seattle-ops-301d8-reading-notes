


## **Readings: Network scanning with NMAP**
Below you will find reading material and additional resources that support today’s topic and the upcoming lecture.

Review the Submission Instructions for guidance on completing and submitting this assignment.

### **Reading For Lecture & Lab**

*What is a Port Scanner and How Does it Work?* 
>A port scanner is a program that tries to see what ports are avaiable on a network and their current status if available.

*What is a port?* 
> A port is a virtual location where networking communication starts and ends

*Describe it with an analogy that would help a family member understand.*
> They are kind of like a network doorway that a port scanner can see if the door is open, if something is going through the door, or if a door appears locked or hidden.

*What does a port scanner send to a port to check the current status?*
>It sends certain types of requests for information and based on the response or lack of response can tell you some information about the target network.

*When a port scanner sends a request to connect, what are the three possible responses? Describe them.*
> 1. **ICMP reply-**
     Indicates that the target is alive. A ping scan is an automated blast of many ICMP echo requests to different targets to see who responds.
> 2. **TCP Half Open-**
    Sometimes referred to as an SYN scan. It’s a fast and sneaky scan that tries to find potential open ports on the target computer. SYN packets request a response from a computer, and an ACK packet is a response. In a typical TCP transaction, there is an  SYN, an ACK from the service, and a third ACK confirming message received.
> 3. **TCP Connect-**
    This port scanning technique is basically the same as the TCP Half-Open scan, but instead of leaving the target hanging, the port scanner completes the TCP connection. It’s not as popular a technique as the TCP half-open. First, you have to send one more packet per scan, which increases the amount of noise you are making on the network. Second, since you complete the target’s connection, you might trip an alarm that the half-open scan wouldn’t.


**What is the difference between TCP and UDP?**
>TCP and UDP are the two most common protocols in use for Internet Protocol (IP) networks. Transmission Control Protocol (TCP) is a nice orderly transaction protocol: TCP sends each packet in order, complete with error checking, verification, and a 3-way handshake to confirm each packet is successful.

>UDP doesn’t have any error checking but tends to be faster. Live streaming and online video games often use UDP for this reason. UDP is a connectionless protocol, so programs that use UDP just send the data – and if you miss a packet, you will never get it again.


### Common Ports 
List and describe the ports used for the following:

Telnet:
>Default Port 44
>>Used connect to the computer running the telnet Server Service

SSH:
>Default Port 22 
>>Secure Shell. The SSH protocol was designed as a secure alternative to unsecured remote shell protocols. It utilizes a client-server paradigm, in which clients and servers communicate via a secure channel.

DNS:
>Default Port 53
>>DNS queries and responses can be transmitted over both UDP (User Datagram Protocol) and TCP (Transmission Control Protocol) on Port 53.
DNS queries are typically sent using UDP on Port 53. UDP is a connectionless protocol that offers fast and lightweight communication. It is suitable for most DNS queries, which are small and do not require guaranteed delivery or ordered transmission.

SMTP:
>Typical Ports: 25, 587, 465, or 2525
>>An SMTP port is a communication endpoint that handles information transfers from one server to another. While SMTP (Simple Mail Transfer Protocol) guarantees most emails are being sent on the web, a port makes sure the right email data is going to the right place.

HTTP:
>Default Port 80
>>In client-server protocols, it is the client which establishes the connection. Opening a connection in HTTP means initiating a connection in the underlying transport layer, usually this is TCP.
With TCP the default port, for an HTTP server on a computer, is port 80. Other ports can also be used, like 8000 or 8080. The URL of a page to fetch contains both the domain name, and the port number, though the latter can be omitted if it is 80. 

HTTPS:
>Default Ports 443, 8443
>>HTTPS ports are dedicated network ports that allow internet users to transmit data via a secure connection encrypted using an SSL/TLS certificate.

RDP:
>Default Port 3389
>>To connect to your PC by using a Remote Desktop client, you're creating a peer-to-peer connection. This means you need direct access to the PC (sometimes called "the host"). If you need to connect to your PC from outside of the network your PC is running on, you need to enable that access.

Ping:
>User defined specific Ports
>>Pinging ports is one of the most effective troubleshooting technique in order to see if a service is alive or not. Used by system administrators on a daily basis, the ping command, relying on the ICMP protocol, retrieves operational information about remote hosts.





References:

https://www.varonis.com/blog/port-scanning-techniques

https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/telnet

https://phoenixnap.com/kb/what-is-ssh

https://www.howtouselinux.com/post/dns-port

https://kinsta.com/blog/smtp-port/

https://developer.mozilla.org/en-US/docs/Web/HTTP/Session

https://www.hostinger.com/tutorials/https-port

https://learn.microsoft.com/en-us/windows-server/remote/remote-desktop-services/clients/remote-desktop-allow-outside-access

https://devconnected.com/how-to-ping-specific-port-number/

