---

layout: post
title: Scapy
categories: [Networking, Python]
image: https://i.ibb.co/C7Vr7DS/pythony.jpg
---

Hey guys and welcome to this sort of tutorial where I will be talking of how we can ease how we look at packets from a very simple python script.

So we will be utilizing a tool called scapy which is used in networking. Okay with that said let us go into it.

## PYTHON SCRIPT

'''python

from scapy.all import *

ps = rdpcap["example.pcap"]

ps[0].show ( )

Basically we are importing scapy and utilising the rdpcap method.

## ANALYSIS

![1](https://i.ibb.co/y0Y6sJp/python.png)

Let us analyze our output.

When we run the code we shall see categories, starting of with the Ethernet category we see ***dst**. 
Basically this is the destination Mac address while the ***src*** is the source mac address. 
And type is ip version.

Next category which is IP. Well we can see a lot in here

***proto** which is the protocol
***src*** which is the source Ip address
***dst** which is the destination ip address

I feel like that is much lighter than using wireshark. What do you think?