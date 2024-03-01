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

![](/image/devops/devops-01.png)

### Encapsulation and Decapsulation

Each layer adds its own header to the message coming from above and the receiving entity on the other end removes it.

Adding the header is called **encapsulation** and removing it is called **decapsulation**.

![](/image/devops/devops-02.png)

There are several models along which computer networks are organized. The two most common ones are **the Open Systems Interconnection (OSI) model** and the **Transmission Control Protocol/Internet Protocol (TCP/IP) model**.

### OSI Model

The model splits up a communication system into 7 abstract layers, stacked upon each other.
Mnemonic: Please Do Not Throw Sausage Pizza Away

![](/image/devops/devops-03.png)

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

![](/image/devops/devops-04.png)

![](/image/devops/devops-05.png)

![](/image/devops/devops-06.png)

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

![](/image/devops/devops-07.png)

Note that HTTP is a stateless protocol: servers do not store any information about clients by default.

Application layer protocols rely on underlying transport layer protocols called UDP (User Diagram Protocol) and TCP (Transmission Control Protocol).

• TCP ensures that messages are always delivered. Messages get delivered in the order that they are sent.

• UDP does not ensure that messages get delivered. This means that some messages may get dropped and so never be received.

There are two kinds of HTTP connections: Non-persistent HTTP connections, Persistent HTTP connections

• Non-persistent HTTP connections use one TCP connection per request.

• Persistent HTTP was developed, which used a single client-server TCP connection for all the HTTP request-responses for a session.

The first line is called the request line, while the rest are called header lines.
https://en.wikipedia.org/wiki/List_of_HTTP_header_fields

![](/image/devops/devops-08.png)

![](/image/devops/devops-09.png)

**Uniform Resource Locators (URLs)** are used to identify an object over the web. A URL has the following format: protocol://hostname:port/path-and-file-name.
HTTP response messages don’t have the URL or the method fields. Those are strictly for request messages.

![](/image/devops/devops-10.png)

• **Connection type** - In this case, indicates that the server will close the TCP connection after it sends the response.

• **Date** - The date at which the response was generated.

• **Server** - Gives server software specification of the server that generated the message. Apache in this case.

• **Last-Modified** - The date on which the object being sent was last modified.

• **Content-Length** - The length of the object being sent in 8-bit bytes.

• **Content-Type** - The type of content. The type of the file is not determined by the file extension of the object, but by this header
The status code comes next which tells the client if the request succeeded or failed.
• 1xx codes fall in the informational category
• 2xx codes fall in the success category
• 3xx codes are for redirection
• 4xx is client error
• 5xx is server error
**cURL (Client URL)** is a command-line tool that transfers data to or from a server.
If you provide a URL without a leading protocol:// scheme, curl guesses what protocol you want. It then defaults to HTTP but assumes others based on often-used host name prefixes.

![](/image/devops/devops-11.png)

• The **--head flag or -I** in short, tells cURL to send an HTTP request with the head method. In other words, the entity-body of the HTTP message is not fetched.

• The **-silent flag** tells cURL to not display the progress meter.

### Cookies

Cookies are unique string identifiers that can be stored on the client’s browser.
These identifiers are set by the server through HTTP headers when the client first navigates to the website.

When a server wants to set a cookie on the client-side, it includes the header Set-cookie: value in the HTTP response.

The cookie file contains:

• The website’s domain

• The string value of the cookie

• The date that the cookie expires (yes, much like actual cookies, they do expire)

### DNS

The most well-known lookup service is the **Domain Name System (DNS)**.

![](/image/devops/devops-12.png)

![](/image/devops/devops-13.png)

Root DNS servers are the first point of contact for a DNS query (after the client’s local cache of names and IP addresses).

**Local DNS Cache** - DNS mappings are often also cached locally on the client end-system to avoid repetitive lookups and saves time for often visited websites. This is done via an entity called the local resolver library, which is part of the OS. The application makes an API call to this library. This library manages the local DNS cache.

The DNS distributed database consists of entities called RRs, or Resource Records.
RRs contain some or all of the following values:

• **Name** of the domain.

• **Resource data (RDATA)** provides information appropriate for the type of resource record.

• **Type** of the resource record. We will discuss these shortly.

• **Time-to-live (TTL)** is how long the record should be cached by the client in seconds.

• **DNS Class** - There are many types of classes but we’re mainly concerned with IN which implies the ‘Internet’ class.

Types of resource records

• **Address** type or A addresses contain IPv4 address to hostname mappings.

• **Canonical** name or CNAME records are records of alias hostnames against actual hostnames. For example, if, ibm.com is really servereast.backup2.com, then the latter is the canonical name of ibm.com.

• **Mail Exchanger** or MX records are records of the server that accepts email on behalf of a certain domain.

## Transport Layer

The network layer (directly below the transport layer) transports messages from one end-system to another, the transport layer delivers the message to and from the relevant application on an end-system.

Other responsibilities of the transport layer -

• Logical application-to-application delivery

• Can allow multiple conversations

• Segments data

• Multiplexes & demultiplexes data

The transport layer and its protocols reside on end-systems.

**Demultiplexing** is the process of delivering the correct packets to the correct applications from one stream.

**Multiplexing** allows messages to be sent to more than one destination host via a single medium.

The transport layer labels packets with the port number of the application a message is from and the one it is addressed to. This is what allows the layer to multiplex and demultiplex data.

• Port numbers are 16-bit long and range from 0 and 65,535.

• The port numbers 0−1023 are reserved for certain applications and are called well-known ports. For example, port 80 is reserved for HTTP.

**Sockets**, which are gateways to applications, are identified by a combination of an IP address and a 16-bit port number.

When more packets than the network has bandwidth for are sent through, some of them start getting dropped and others get delayed. This phenomenon leads to an overall drop in performance and is called **congestion**.

• Congestion physically occurs at the network layer (i.e., in routers)
Bandwidth cannot be divided and allocated equally amongst end-systems!
**Congestion collapse** occurs when all end-systems are sending a lot of traffic but nothing is being received, for example, when all or most packets are dropped. There are few causes for this, including but not limited to **Spurious retransmissions**.

To avoid congestion, on average, the sum of the transmission rate allocated to all hosts at any given time should be less than or equal to the bottleneck link’s bandwidth.

There are three types of imperfections that must be considered by the transport layer:

• Segments can be corrupted by transmission errors.

o The simplest error detection scheme is the checksum.

• Segments can be lost.

o Since the receiver sends an acknowledgment segment after having received each data segment, the simplest solution to deal with losses is to use a retransmission timer.

• Segments can be reordered or duplicated.

o To identify duplicates, transport protocols associate an identification number with each segment called the sequence number.

**UDP, or User Diagram Protocol**, is a transport layer protocol that works over the network layer’s famous Internet protocol.

UDP does not involve any initial handshaking like TCP does and is hence called a connectionless (no established connection between hosts) protocol.
Other than the headers, a UDP datagram contains a body of data which can be up to 65,528 bytes long.

---
