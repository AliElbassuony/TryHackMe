<div align="center">

![Network Fundmentals](https://github.com/AliElbassuony/TryHackMe/blob/main/images/4.jpg)

</div>

<h1 align="center"> Network Fundmentals </h1>

<div align="center">

![7%](https://progress-bar.dev/7/?title=Progress)

</div>

## What is Networking?

- Simply things connected

- A Network can be formed by anywhere from 2 devices to billions

- An Essential concept to grasp in cybersecurity.

## What is the Internet?

- The Internet is one giant network that consists of many, many small networks within itself

<div align="center">

![The Internet](https://assets.tryhackme.com/additional/networking-fundamentals/intro-to-networking/what-is-the-internet/internet2.png)

</div>

- the Internet is made up of many small networks all joined together.
- Small networks are called `private networks`
- Networks connecting these small networks are called `public networks` or the Internet

- Network can be one of two types:

  - A private network
  - A public network

## What’s difference between The Internet and The Web?

|                                          | The Internet               | The Web                                                                               |
| ---------------------------------------- | -------------------------- | ------------------------------------------------------------------------------------- |
| refer to                                 | global network of networks | World Wide Web (www) is a collection of information that is accessed via the Internet |
| Another way                              | infrastructure             | is served on top of that infrastructure                                               |
| can be viewed as a                       | big book store             | collection of books on that store                                                     |
| At a high level, we can even think of as | hardware                   | software                                                                              |

```
The first iteration of the Internet was within the ARPANET project in the late 1960s.
This project was funded by the United States Defence Department and was the first documented network in action.
it wasn't until 1989 when the Internet as we know it was invented by Tim Berners-Lee by the creation of the World Wide Web (WWW).
```

## Identifying Devices on a Network

- To communicate and maintain order, devices must be both identifying and identifiable on a network.

- two means of identification, with one being permeable. These are:

  - An IP Address
  - A Media Access Control (MAC) Address -- think of this as being similar to a serial number.

<div align="center">

![Addresses](https://assets.tryhackme.com/additional/cmn-aoc2020/day-8/1.png)

</div>

### IP Addresses

- IP (Internet Protocol) addess can be used as a way of identifying a host on a network for a period of time

- IP address can then be associated with another device without the IP address changing

<div align="center">

![IP Address](https://assets.tryhackme.com/additional/networking-fundamentals/intro-to-networking/what-is-a-network/octets.png)

</div>

- IP address is a set of numbers that are divided into `4 octets`

- Value of each octet will be the IP address of the device on the network. This number is calculated through `IP addressing & subnetting`

- IP addresses can change from device to device but cannot be active simultaneously more than once within the same network.

#### IP Addresses & Protocols

- IP Addresses follow a set of standards known as `protocols`

- `Protocols` are the backbone of networking and force many devices to communicate in the same language

- devices can be on both a private and public network

- A public address is used to identify the device on the Internet, whereas a private address is used to identify a device amongst other devices

- Public IP addresses are given by your Internet Service Provider (or ISP) at a monthly fee (your bill!)

#### IP addresses Versions

- As more and more devices become connected increasingly harder to get a public address approximately 50 billion devices connected on the Internet by the end of 2021

- IPv4 uses a numbering system of 2^32 IP addresses (4.29 billion)

- IPv6 is a new iteration of the Internet Protocol addressing scheme to help tackle this issue. it boasts a few benefits:
  - Supports up to 2^128 of IP addresses (340 trillion-plus)
  - More efficient due to new methodologies

## MAC Addresses

- Devices on a network will all have a physical network interface, which is a microchip board found on the device's motherboard

- This network interface is assigned a unique address at the factory it was built at, called a MAC (Media Access Control ) address.

- The MAC address is a `12 character` hexadecimal number split into two's and separated by a colon

- The first 6 characters represent the company that made the network interface, and the last 6 is a unique number.

<div align="center">

![MAC Address](https://assets.tryhackme.com/additional/networking-fundamentals/intro-to-networking/what-is-a-network/mac_address.png)

</div>

- an interesting thing with MAC addresses is that they can be faked or "spoofed" in a process known as spoofing.

- This spoofing occurs when a networked device pretends to identify as another using its MAC address.

- When this occurs, it can often break poorly implemented security designs that assume that devices talking on a network are trustworthy.

## Ping (ICMP)

- The Most Fundmental Network tools availble to us.
- Ping uses `ICMP (Internet Control Message Protocol)` packets
- to Determine performance of a connection betwen devices if connection exist or reliable

<div align="center">

![Ping ICMP](https://assets.tryhackme.com/additional/networking-fundamentals/intro-to-networking/ping/ping1.png)

</div>

- time taken for ICMP packets travelling between devices is measured by ping

- measuring is done using ICMP's echo packet and then ICMP's echo reply from the target device.

- Pings can be performed against devices on a network, such as your home network or resources like websites

- `ping IP address or website URL`

----

## Introducing LAN Topologies

### Local Area Network (LAN) Topologies

- Experimentation and implementation of various network designs.

- The term `topology`, we are actually referring to the design or look of the network at hand.

#### Star Topology

- Devices are individually connected via a central networking device such as a switch or hub
- The most commonly found today because of its reliability and scalability - despite the cost.
- Any information sent to a device in this topology is sent via the central device to which it connects.

#### Bus Topology
----

### Broadcasting

- in computer network is a group communication, where a sender sends data to receivers simultaneously.

### VLAN (Virtual Local Area Network)

- The computers, servers, and other network devices are logically connected regardless of their physical location.

- Benefits of VLAN:
  - Traffic Management
  - make a network simpler
  - improved security

### HTTP 
- Hypertext Transfer Protocol (HTTP) is the protocol that specifies how a web browser and a web server communicate. Your web browser requests content from the website web server using the HTTP protocol usually using port 80.
- the set of rules used for communicating with web servers for the transmitting of webpage data, whether that is HTML, Images, Videos, etc.

### HTTPS
- HTTPS is the secure version of HTTP usually using port 443.
- HTTPS data is encrypted so it not only stops people from seeing the data you are receiving and sending.
- it also gives you assurances that you're talking to the correct web server and not something impersonating it.

###  URL (Uniform Resource Locator)
- 
