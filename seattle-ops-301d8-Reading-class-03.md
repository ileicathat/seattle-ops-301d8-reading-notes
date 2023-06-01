Readings: Network Segmentation

Below you will find reading material and additional resources that support today’s topic and the upcoming lecture.

Review the Submission Instructions for guidance on completing and submitting this assignment.

Reading
CIDR Block Notation Explained in 2 Minutes

### What is CIDR notation? a CIDR block?
>CIDR notation is a way of representing a CIDR block, which is simply a range of IP addresses. When you create a network, the aim is to make sure there are enough available IP addresses for your use case, without making the CIDR block too large and wasteful.

### How many octets are found in an IPv4 address?
>4

### Setting binary aside and using the decimal system, what is the range of numbers found in an octet?
>0-255

### What does the final digit after the “/” represent in an IPv4 address?
>The number of bits that make up the mask

How many IP addresses are in the CIDR block 10.0.0.0/24?
What Is Network Segmentation and Why It Matters?
> 256

>Useful for organizing subnets

In your own words, describe network segmentation.
> It is a method similar to Russian nesting dolls. Where each layer of a network as you go deeper into a system is secured by needing different levels of access privileges 


Network segmentation isn’t important as long as the network is using a well configured firewall. Do you agree? Why or why not?
>Firewalls can be penetrated in different ways, some as easy as someone unknowingly giving the bad party access directly. But with segmentation, what that person is able to access is limited unless they acquire yet more permissions.

What is a screened subnet?
> This is a way of keeping things that the public can see and interact with separate from other more sensitve data or access on the LAN

Cameras, ID card scanners, locked doors and biometrics are just a few examples of what type of security?
> Traditional Physical Security
Videos
Classful Subnetting

VLANs and Trunking