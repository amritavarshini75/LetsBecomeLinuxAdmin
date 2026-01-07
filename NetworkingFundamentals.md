# Networking Fundamentals

## IP Address
* The IP Address is basically a unique address assigned to a particular device. Basically, how every house has a home address for identification or delivery purpose - similarly every device will also have a unique address assigned to it. This makes it easier to identify a device
* The standard for address allocation is either done through IPv4 or IPv6. Lets dive deeper into these later.
* Using IPv4 you can generate many unique addresses and assign each of them to a device.
* The standard IP address format for the devices is IPv4 standard
* An IPv4 address standard looks like x.x.x.x eg: 10.1.1.12 or 172.1.1.12

## ipconfig/ ifconfig command
```bash
ipconfig
ifconfig
````
* These commands are used to know the IP address of your device / linux server

## IPv4
<img width="282" height="131" alt="image" src="https://github.com/user-attachments/assets/d71bfdcc-6b4c-4d60-af8a-044f2bad0085"/>
* These many IP addresses can be created using a IPv4 IP address standard

<img width="463" height="217" alt="image" src="https://github.com/user-attachments/assets/9ebed109-f78a-42a5-8e8d-56e1bd2a17c9" />
* each x - 0 - 255 (It represents 1 Byte = 8 Bits)
* So an IPv4 IP address consists of 4 bytes and 32 bits.

<img width="446" height="112" alt="image" src="https://github.com/user-attachments/assets/23b73b77-b7b5-4235-920a-4feec0f92d2c" />
* IP Address to Binary conversion example

## Subnetting
* The concept of breaking down a IP Range into parts and using them for different purposes is called subnetting. It helps us to create a secure network with in a IP Range. 
* If there's a IP Range say 10.3.2.1/20 - you can divide this range into sub ranges and that particular subrange is called a subnet.
* Usually subnetting can be done for VPC CIDR range and Classic/ On Prem Infrastructure dedicated IP Range.
* For VPC CIDR Range - The user will get to decide the CIDR range and will have full control over the IP Range and the subnets
* For On Prem or Classic Infra - The Cloud Provider or a Provider will provide you a dedicated IP range which usually covers some extra IP addresses compared to the VPC and you will have control over the IP Range provided to you by the provider.

*  Advantages of using subnet: It provides security, privacy and isolated network.

You can create a subnet in home network as well.

Types of subnets
Private subnet -> This network does not have access to internet
Public subnet->  This network has access to internet



  BTW , how do you provide access to internet for a subnet?
by attaching the route tables to the network and the destination in the route table must be internet gateway - will dive deeper into this later

Whenever you are subnetting a network you will basically be giving an IP Range (Range of IP addresses or number of IP addresses present within that network) - This is called CIDR range. Also note that whenever are subnetting you will be asked to provide a CIDR range.

Note : most of the private subnets IP's start with - 192,172 or 10 (This is a best practice)

Ports:

Long explanation but bear with me
So basically computers or servers have different kinds of services that are running. Now, the computer if no port concept is in place we don't know which service is running where- here lets use a analogy of tv channels. once you switch on the tv you know that TV will have dedicated channel number for disney and another for mtv. similarly to identify a service running on a server we have numbers called ports. so you can relate like tv channels have channel numbers whereas services running on a server or computer have ports. The tv channels are decided upon and it is slightly more complicated but ports is something engineers invented themselves and agreed upon. so for example to access a service on a server we use server ip and port. eg: 10.1.1.1:8080 - something like this

usually there are 65536 port numbers in the word
1-1023 are reserved for well-known services.
eg: 443 - HTTPS, 22-SSH etc

so when a server/computer receives incoming traffic dedicated to a particular service - that traffic is routed to that particular service using the port dedicated to it.







