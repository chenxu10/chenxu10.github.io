---
layout: post
title:  "Teach Yourself DeFi: From Client-Server to P2P Protocol"
date:   2022-03-05 16:45:30 -0500
categories: datascience
---
The whole web2 economy is built in a client-server model. Big techs like Google, Facebook, Amazon, and Linkedin all use a central server to provide services. In the meantime, clients request data or write information into it.

A client-server architecture is innately centralized and thus has a single point of failure. Once the server is down, hacked, or censored, all clients are negatively impacted. 

![clientserver](/images/clientserver.png)

In contrast, A P2P network is a distributed networking protocol, in which the central server is killed. This indicates each peer in this protocol needs not only to get data but also to post data to the network. You can see it as a model of people gossiping in a village to pass a rumor or virus mutating and propagating in the pandemic.

![peer2peer](/images/peer2peer.png)

## Why did Satoshi choose P2P for Bitcoin?

When Satoshi created a digital cash system, he used the P2P protocol because of two nice properties in it.

First, P2P is leaderless and decentralized. But decentralization is just a means to an end. It gives a strong resistance to censorship. Imagine you want to censor the whole network, you will need to have huge computation power to make every node collude.

Second, the P2P protocol is more fault tolerance. Even if one node fails, the whole network is still functioning. In each cluster, machines fail far more frequently than you imagine. For example, A 50 percent chance that the cluster will overheat in Google's data center provided by Google fellow Jeff Dean.

## History of P2P Protocol

The P2P Protocol was first designed to coordinate enormous computation tasks across distributed computational resources. The idea became popularized in 1999 by the success of Napster, a file-sharing system where people can download music freely from any other peer in the network.

Today P2P is still the most fundamental protocol of file sharing, dominated by the major player BitTorrent. Unlike Napster, Bit is still flourishing and responsible for around 70% of web traffic for mainly two reasons:

First, BitTorrent adopts a tit for tat model on bandwidth sharing. Tit for tat is a strategy that will help the ecosystem reach an evolution stable environment illustrated by Robert Axelrod's classic work in 'The Evolution of Cooperation. It punishes the user trying to exploit the system by taking a free ride and encourages the users who pay in advance.

Second, it managed to brand itself as a better way for innocuous file sharing like Unix distribution updating. It also did its best to prevent copyrighted file sharing.

## How can you teach yourself P2P networking?

From a data structure perspective, web3's foundation blockchains are nothing more than linked lists with hashed functions. From a networking perspective, blockchains are further development of P2P networks.

In order to understand how P2P works, you will need to understand:

- [x] Internet Routing and how Internet works

Try `ping yuba.stanford.edu` and `traceroute yuba.stanford.edu`. You will find what paths information packets take and how long does it take to travel back and forth between the start place and California.

- [x] [TCP vs UDP](https://www.diffen.com/difference/TCP_vs_UDP)

TCP is a connection-oriented protocol and UDP is a connectionless one. UDP is faster, used more in video streaming, gaming, and live broadcasts. But it cannot guarantee the delivery of the packet and packets don't necessarily arrive in order like TCP.

- [x] [Packets, Routers, and reliability](https://www.youtube.com/watch?v=aD_yi5VjF78)

The best way to learn these concepts is by listening to the 'Father of Internet' Vint Cerf explaining those concepts himself. Data are broken into packets with IP addresses indicating their destinations. Routers play roles of data management or you can think of them as traffic managers on the road to keep packets moving through the network smoothly.

- [x] [Gossip protocols and flooding](https://en.wikipedia.org/wiki/Flooding_(computer_networking))

Public blockchains usually spread messages by gossip protocols. The main algorithm used in this protocol is called flooding. Flooding means every incoming packet is sent through every outgoing link except the one it arrived on.

If you need a deep dive into networking, Stanford CS 144 is a great open-source course of choice.

## P2P in the space of Defi

An interesting application of P2P protocols in real world are DeFi(Decentralized Finance) Protocols. In the past two years, both the trading volume and total amount of value of DeFi space has reached 3 billion daily and 76.3 billion. It leverages P2P protocols and distributed ledgers to remove the centralized control banks. I listed some representative emerging markets and their corresponding new companies in below.

### Insurance Market: [InsurAce.io](https://files.insurace.io/public/InsurAceWhitepaper.pdf)

InsurAce.io is a decentralized insurance protocol, providing reliable safe insurance to protect clients' crypto anonymously. 

It provides two functional arms very much like traditional insurance company, the insurance arm and investment arm. The free capital in the insurance capital pool can be placed into the investment pool to gain higher yield, while the insurance arm will provide protection to the investment activities. Meanwhile, the yield at the investment side will in turn complement the premium at the insurance side, and further reduce the cover cost for customers.

Sources of profit are coming from a portion of carry from the investment returns and revenues from the insurance premium.

### Lending Market: [Compound](https://compound.finance/documents/Compound.Whitepaper.pdf)

Compound is a protocol that enables you to get a loan from a smart contract without paperwork. Or you can use it to lend crypto to earn interest. It makes money not by directly charging your service but by taking interests fee from the customer's funds.

### Exchange Market: [UNISWAP](https://uniswap.org/whitepaper.pdf)

UNISWAP enables you to swap any blockchain asset for any other. UNISWAP makes profit by charging a proportion of transaction fees.

### Stable Coin Market: [MAKER DAO](https://makerdao.com/es/whitepaper/)

MakerDAO is a decentralized organization dedicated to bringing stability to the cryptocurrency economy. It allows you to get synthetic US dollars. MAKER DAO's revenues are coming from accrued stability fees and liquidation penalities.


## Problem Sets

- Try using python NetworkX package to draw a client-server model and a P2P model.
- Design a class which can spread the message of current favorite books in a community.
- Think of a case where DeFi can revolutionize one sector in finance industry in the next 6 months.
