Justin R. Dotson

Seattle ops 301d8 

Readings: Network Address Translation
Below you will find reading material and additional resources that support today’s topic and the upcoming lecture.

Review the Submission Instructions for guidance on completing and submitting this assignment.

Reading

## Network Address Translation (NAT)

### What is the main purpose for implementing NAT on a network?
> To conserve internet address space
### At what layer of the OSI model does NAT happen?
> Layer 3
### What happens to packets when NAT runs out of addresses in the pool of available IPs?
> 1. Packet Dropping
> 2. Reuse previously allocated IP address not currently in use
> 3. Multiplex connections through a single public IP (PAT)
### What disadvantage does using NAT pose for routers?
> Increases processing needs, can make troubleshooting more challenging. It relies on having a big enough public address pool to pull from. 

Videos
Network Address Translation (NAT)
Common Network Types
IPv4 and IPv6 Addressing