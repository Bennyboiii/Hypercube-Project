# HYPERSTACK COMPATIBILITY LAYER GROUP VERSION 1

AUTHOR: BEN
DATE: FEB 5 2022
WORKGROUP: MASKEYES

TABLE OF CONTENTS

1.1		ABSTRACT
1.2		IDENTIFYING THE PROBLEM
1.3		BASIC DESIGN

2.1		FRAMEWORK
2.2		INTEGRATION

3.1		DEVICE MANAGEMENT
3.2		USER EXPERIENCE
--NOT FINAL--

ABSTRACT                              1.1

HYPERSTACK is an API that links various front end engine-level graphics and data management libraries with real-time backend information. In theory, HYPERSTACK would act much like Hypertext does currently with webservers. Hypertext interfaces with many extensions such as Javascript, WebGL, WASM, and other Web 2.0 technologies which many sites rely on. HYPERSTACK, however, operates at a lower level than Hypertext does. It can interface with hypertext, but it works in between basic network transfer protocols like TCP and UDP, and networks like TOR and i2p. It routes all compatible protocol information from these networks, and translates them into a common language. Developers can then use this common language to develop apps for HYPERSTACK, without having to choose between protocols and networks. Take the analogy of a plumbing manifold. TOR and i2p use different pipe formats to send water through their respective systems, but HYPERSTACK would be able to screw into both of these systems, and transfer liquid between them. The liquid inside these pipes would be all the same within the manifold, even if it was different in each pipe. HYPERSTACK bridges gaps between darknets and dark protocols, and makes them clear, common and compatible with present web-compatible languages like WASM and Javascript.

IDENTIFYING THE PROBLEM	              1.2

Anyone taking a look at the present state of the web has probably noticed one thing. It has been pretty much overrun by large tech companies relying on the data trade like Google. Presently, Most mainstream internet services are built by Google. And if they aren’t, they are probably built with technologies that Google had a huge part in building. But the issue with the web isn’t the presence of Google itself. The issues lie in the predatory actions large corporations have used against users of the entire web. These include the unauthorized access and trading of personal information, Digital Rights Media, targeted advertisement, media as a service, and much more. The fact that Google runs advertisements on even the most private sites, and that sites like facebook can directly link your personal credit card information to their payment services is enough to scare anyone away. 
	Most people value their privacy, and this has recently been proven by Apple. After implementing a feature that blocks website telemetry upon request, companies that rely on the buying and selling of information have lost much of their stock. If similar features were implemented on other proprietary software, these large companies would take an even greater hit. What most people need, however, is not a hobbyist darknet used to post web1.0 style blogs and storefronts. It is a full decentralized service meant to run faster, real time applications on many different types of hardware, from old flatscreen computers and phones, to XR headsets and glasses. A fully interoperable clearnet, whose services can be easily adopted by the end-user. 	However, there are major concerns and differences in opinion when it comes to what model to use, especially when it comes to p2p services. Many web3 enthusiasts call for a Blockchain. This technology uses an append-only ledger, that handles the transmission of information using cryptographic transactions. This model is widely adopted for cryptocurrencies and online marketplaces, however it has major flaws in it’s security and functionality that have a root in the nature of the model itself. A common alternative is TOR. This is a darknet that sends information through sets of relays, which make it harder for anybody to see your information. However, TOR uses older protocols that don’t necessarily fit with it’s intense method of operation. In terms of p2p technology, i2p is probably the closest we have come to a balanced model. It uses a combination of TCP and UDP to send information through it’s node tree. It also uses software routing to pass information on. This has two major advantages when it comes to decentralization. One, it doesn’t rely on a small community of relays like TOR. Every user acts like a node, each one speeding up and increasing the quality of information transmission on the network. Two, contribution to the network is determined solely by network speed, not computer processing speed like the Blockchain. This means less power is consumed, and larger facilities with more resources don’t control a disproportionate amount of information, which would lead to service blackouts. In fact, this way of transfering data is more akin to torrenting and p2p file sharing. The difference is the hosting service. Like .onion, i2p has a hosting service under domains using the .i2p extension.
  
IDENTIFYING THE PROBLEM	              1.2

Whatever method of p2p data transfer gets adopted, there will always be problems surrounding interoperability. This means that TOR services will not be able to communicate well with i2p services, data on Hyperdrives won’t be able to easily communicate with IPFS drives, and most blockchains won’t be able to communicate with each other. However, the majority of Web 3.0 developers and community members imagine one interconnected network of peers, just like how Hyperlinks transfer users from one piece of hypertext media to another.

HYPERSTACK seeks to bridge these gaps using compatibility layers. This is an API that links various networks and protocols together that would otherwise never reach each other. HYPERSTACK would also adapt this media to many different HCI’s such as desktops, laptops, mobiles, VR/XR headsets, and various AR applications. This can be only be emulated with much difficulty by the end-user, and issues pertaining to security would arise quickly. For example, it is possible to interoperate TOR and i2p using a dynamic proxy, however this would lead to decreased security in the TOR network, and slower speeds in general. HYPERSTACK attempts to fix these issues, while making the experience seamless and effortless for the end-user.

In theory, HYPERSTACK would act much like Hypertext does currently with the classic webserver model. Hypertext interfaces with many extensions such as javascript, WebGL, WASM, and other Web 2.0 technologies which many sites rely on. HYPERSTACK, however, operates at a lower level than Hypertext does. It can interface with hypertext and all of its extensions, but it works in between basic network transfer protocols like TCP and UDP, and networks like TOR and i2p. It routes all compatible protocol information from these networks, and translates them into a common language. Developers can then use this common language to develop apps for HYPERSTACK, without having to choose between protocols and networks. Take the analogy of a plumbing manifold. TOR and i2p use different pipe formats to send water through their respective systems, but HYPERSTACK would be able to screw into both of these systems, and transfer liquid between them. The liquid inside these pipes would be all the same within the manifold, even if it was different in each pipe. HYPERSTACK bridges gaps between darknets and dark protocols, and makes them clear and common.

BASIC DESIGN												    1.3

The main focus of HYPERSTACK is balancing speed, security and interoperability with many different interfaces and protocols. Networks such as the clearnet, TOR, Blockchain, i2p, Hypercore, Usenet, Gnunet, IPFS, Gemini and other p2p projects would be compatible with HYPERSTACK, and intefaces such as CLI, GUI, flatscreen, mobile, VR, AR, HUD and much more would be compatible with applications using HYPERSTACK.


Below is a graphic representation of a HYPERSTACK stack.
![stack](https://user-images.githubusercontent.com/32402247/153954828-b88fc1bb-1bfa-411e-962e-c23effb4512b.png)

FRAMEWORK													    2.1

PART ONE: I/O COMPATIBILITY LAYER 

Many new technologies that are emerging currently have very unique ways of interfacing with computer programs. Most current online interaction is done on flatscreen, keyboard and mouse/trackpad. This resuls in newer interfaces like VR and AR headsets having to adapt to the flatsceen standard. Methods of input and output with these new interfaces also have to adapt, making navigation clunky, and output limited. HYPERSTACK seeks to take advantage of the unique properties of each HCI, and adapt the software for that interface. HYPERSTACK will achieve this by using a separate set of tools for each type of interface. However, this does not mean that multiple binaries need to be created for each HCI. HYPERSTACK will allow multiple methods of input, making switching between different methods of I/O seamless and easy to develop. HYPERSTACK seeks to bridge the gap between standard libraries like libinput and newer ones like OpenXR. HYPERSTACK will also be designed with as much overlap between I/O methods as possible, reducing program redundancy and increasing speed. Since the HYPERSTACK I/O compatibility layer falls between software I/O and the web engine, HYPERSTACK will be designed with web engines in mind, and feature a plethora of navigation tools, 2d and 3d rendering engines compatible with current web graphics languages, and optimizations for the multiple protocols passing through the network, such as changing the network protocol based on frequency of information.

V1 - CONTD

FRAMEWORK													    2.1

PART TWO: PROTOCOL COMPATIBILITY LAYER

Current web engines are compatible with multiple protocols, such as HTTP, FTP and files on your computer. However, these are all web-server based protocols, and any other protocol used (i.e magnet://) usually links to an external program. HYPERSTACK seeks default compatibility with more P2P based protocols like Hypercore, IPFS and Gemini. This will allow more freedom when browsing P2P services, and will make cloud services more affordable, if not completely free. At this level, HYPERSTACK also encrypts, decrypts and checks data so data from vulnerable networks like the blockchain don’t cause the user any harm.

MASSIVE MULTIUSER STORAGE NETWORK

Using IPFS, or a peer to peer fast storage solution similar to IPFS, people who subscribe to a certain service on the network can access a dynamic IPFS storage system that the service creator populates with service programs. This works similarily to .i2p or .onion sites, except with a larger data capacity.
These networks are absolutely separated from each other to prevent cross-infection if it happens. Of course, this doesn’t happen literally. Literal decentralized models still have security issues, so IPFS and similar technologies use a distributed model to increase security and stability across the network.

V1 - CONT’D

FRAMEWORK													    2.1

PART THREE: NETWORK COMPATIBILITY LAYER

The topmost layer of the stack is the one that interfaces with P2P networks by creating a software router. This means that your computer will act like a node for the network you are using at any given moment. Depending on the network, this implementation is either incredibly easy or incredibly hard, on networks like i2p, they supply their own daemon that easily interfaces with web engines already. However, networks like TOR are more complicated. They use a TOR client, meaning that you connect to TOR the same way you connect to a clearnet webserver. You communicate by giving and receiving information only you are entitled to, and not by passing your information through the network along with any adjacent node’s information. If you use a TOR relay, they are often separate machines. These two models are the most common, and HYPERSTACK will adapt to both and more. HYPERSTACK will first create a software router and rout as much P2P traffic through it as possible to establish a good connection with the network. It will then create a proxy for each network and multiplex all networks being visited currently. This avoids the hassle of setting up a dynamic proxy, or using multiple profiles with multiple different proxies. It will also separate the networks so you aren’t running a network inside another network, which can happen if a network uses many outproxies, like TOR.



V1 - CONT’D 
