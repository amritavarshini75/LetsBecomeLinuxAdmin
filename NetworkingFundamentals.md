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







