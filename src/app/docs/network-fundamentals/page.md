---
title: Network Fundamentals
nextjs:
  metadata:
    title: Network Fundamentals
    description: Quidem magni aut exercitationem maxime rerum eos.
---

## Internet and the OSI Model

A **network** is officially defined as a group or system of interconnected people or items.
**internet** vs. **Internet** An internet with a lowercase “i” is any interconnection of computer networks. Whereas the global Internet is always spelled with a capital I.

**Layered architectures** give us modularity by allowing us to discuss specific, well-defined parts of larger systems.

Computer networks are conceptually divided into layers that each serves the layer above and below it.

The top layer in most layered models is called the **application layer**.

With **Horizontal Layers** in Networks, applications in the application layer are seemingly communicating with each other directly or horizontally. They are not aware of the layer below.

### Encapsulation and Decapsulation

Each layer adds its own header to the message coming from above and the receiving entity on the other end removes it.

Adding the header is called **encapsulation** and removing it is called **decapsulation**.

There are several models along which computer networks are organized. The two most common ones are **the Open Systems Interconnection (OSI) model** and the **Transmission Control Protocol/Internet Protocol (TCP/IP) model**.

### OSI Model

The model splits up a communication system into 7 abstract layers, stacked upon each other.
Mnemonic: Please Do Not Throw Sausage Pizza Away

**Application Layer** - End-users interact with the application layer. Layer 8 is a pseudo-layer for the end user.

**Presentation Layer** – Presents data (encoding), Encryption, Abstracts, End-to-End compression
**Session Layer** - The session layer must manage the mapping of messages delivered by the transport layer to the sessions.

**Transport Layer** - the transport layer segments it into smaller chunks. These chunks are called datagrams or segments depending on the protocol used. The transport layer adds this information to the segment/datagram.

**Network Layer** - They facilitate the transportation of packets from one end system to another and help to determine the best routes that messages should take from one end system to another. Routing protocols, Load Balancing.

**Data Link Layer** - encapsulates packets for transmission across a single link, resolves transmission conflicts, handles addressing, multiplexing & demultiplexing.

**Physical Layer** - Provides a solid electrical and mechanical medium to transmit the data.

### TCP/IP Model

The TCP/IP Model is also known as the Internet protocol suite.

Its development was funded by DARPA (Defense Advanced Research Projects Agency).

The TCP/IP model splits up a communication system into 5 abstract layers, stacked upon each other. Each layer performs a particular service and communicates with the layers above and below itself.

---

## Application Layer

• Writing data off to the network in a format that is compliant with the protocol in use.

• Reading data from the end-user.

• Providing useful applications to end users.

• It carries messages to the transport layer.

### Client-Server Architecture

Network application’s architecture – refers to how applications are structured across end systems.

In this architecture, a network application consists of two parts: client-side software and server-side software. These pieces of software are generally called processes, and they communicate with each other through messages.

### Peer-to-Peer Architecture (P2P)

In this architecture, applications on end-systems called ‘peers’ communicate with each other. No dedicated server or large data center is involved.

The key advantage of the P2P architecture is that it can scale rapidly.

Regardless of P2P’s decentralized nature, each peer can be categorized as servers or clients i.e., every machine is capable of being a client as well as a server.

A lot of popular applications today, like BitTorrent, are based on P2P architectures.

### Program vs. Process vs. Thread

• A program is simply an executable file. An application such as MS Word is one example.

• A process is any currently running instance of a program. So, one program can have several copies of it running at once. One MS Word program can have multiple open windows.

• A thread is a lightweight process. One process can have multiple running threads. The difference between threads and processes is that threads do lightweight singular jobs.

### Sockets

Processes on different machines send messages to each other through the computer network. The interface between a process and the computer network is called a socket.

Note that sockets do not have anything to do with hardware – they are software interfaces.

It is a combination of the IP address and a port number.

### Addressing

Since every end-system may have a number of applications running, ports are used to address the packet to specific applications.

Some ports are reserved such as port 80 for HTTP and port 443 for HTTPS.

The port that an application will use is usually predefined by its application developers.

An ephemeral port is a communications endpoint (port) of a transport layer protocol of the Internet protocol suite that is used for only a short period of time for the duration of a communication session.

With ephemeral port, different port numbers are dynamically generated for each instance of an application. The port is freed once the application is done using it.

### HTTP

Web pages are objects that consist of other objects. The base object of a web page is often an HTML file that has references to other objects by making requests for them via their URL.

HTML or HyperText Markup Language is the standard markup language to build webpages.

A URL, or Universal Resource Locator, is used to locate files that exist on servers.

URLs consist of the following parts: protocol in use, the hostname of the server, the location of the file, arguments to the file.

Note that HTTP is a stateless protocol: servers do not store any information about clients by default.

Application layer protocols rely on underlying transport layer protocols called UDP (User Diagram Protocol) and TCP (Transmission Control Protocol).

• TCP ensures that messages are always delivered. Messages get delivered in the order that they are sent.

• UDP does not ensure that messages get delivered. This means that some messages may get dropped and so never be received.

There are two kinds of HTTP connections: Non-persistent HTTP connections, Persistent HTTP connections

• Non-persistent HTTP connections use one TCP connection per request.

• Persistent HTTP was developed, which used a single client-server TCP connection for all the HTTP request-responses for a session.

---

## Vitae laborum maiores

Sit commodi iste iure molestias qui amet voluptatem sed quaerat. Nostrum aut pariatur. Sint ipsa praesentium dolor error cumque velit tenetur.

### Corporis exercitationem

Sit commodi iste iure molestias qui amet voluptatem sed quaerat. Nostrum aut pariatur. Sint ipsa praesentium dolor error cumque velit tenetur quaerat exercitationem. Consequatur et cum atque mollitia qui quia necessitatibus.

Possimus saepe veritatis sint nobis et quam eos. Architecto consequatur odit perferendis fuga eveniet possimus rerum cumque. Ea deleniti voluptatum deserunt voluptatibus ut non iste. Provident nam asperiores vel laboriosam omnis ducimus enim nesciunt quaerat. Minus tempora cupiditate est quod.

### Reprehenderit magni

Sit commodi iste iure molestias qui amet voluptatem sed quaerat. Nostrum aut pariatur. Sint ipsa praesentium dolor error cumque velit tenetur quaerat exercitationem. Consequatur et cum atque mollitia qui quia necessitatibus.

Voluptas beatae omnis omnis voluptas. Cum architecto ab sit ad eaque quas quia distinctio. Molestiae aperiam qui quis deleniti soluta quia qui. Dolores nostrum blanditiis libero optio id. Mollitia ad et asperiores quas saepe alias.
