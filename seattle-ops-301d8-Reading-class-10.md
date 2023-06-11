Justin R. Dotson

06-12-23

Readings: VPC
Below you will find reading material and additional resources that support today’s topic and the upcoming lecture.

## After you’ve completed the reading, answer the following:

### How can one host within a VPC any services that need to be public?
> By using Subnets, VLAN, VPN A VPC will have a dedicated subnet and VLAN that are only accessible by the VPC customer. This prevents anyone else within the public cloud from accessing computing resources within the VPC – effectively placing the "Reserved" sign on the table. The VPC customer connects via VPN to their VPC, so that data passing into and out of the VPC is not visible to other public cloud users.


### What are examples of services that would live in the publicly-accessible part of the VPC? The privately-accessible part?
>Public - AWS, Google Cloud Platform, and Microsoft Azure

>Private- a corporations different departments hosted on a service like AWS but each department has access only to thier individual resources but the different departments not having access to each others without specific permissions being granted.

### What are the trade-offs of using a VPC vs traditional infrastructure?
>Scalability: Because a VPC is hosted by a public cloud provider, customers can add more computing resources on demand.

>Easy hybrid cloud deployment: It's relatively simple to connect a VPC to a public cloud or to on-premises infrastructure via the VPN. (Learn about hybrid clouds and their advantages.)

>Better performance: Cloud-hosted websites and applications typically perform better than those hosted on local on-premises servers.

>Better security: The public cloud providers that offer VPCs often have more resources for updating and maintaining the infrastructure, especially for small and mid-market businesses. For large enterprises or any companies that face extremely tight data security regulations, this is less of an advantage.

Reading
What is a Virtual Private Cloud(VPC)