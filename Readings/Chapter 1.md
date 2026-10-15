## Introduction to networking
#chapter-1
# What is Network?

A computer network can be described as a system of interconnected devices that can communicate using some common standards called the **[Internet protocol suite]** or **[TCP/IP]**. These devices communicate to exchange network resources, such as files and printers, and network services.

Here is an example of a computer network consisting of two computers connected together:

[![what is network](https://study-ccna.com/wp-content/images/network_of_two_computers_only.jpg "network of two computers only")](https://study-ccna.com/wp-content/images/network_of_two_computers_only.jpg)

The example above shows that the two computers are directly connected using a cable. This small network can exchange data between just these two computers.

What if we want to expand our network? Then we can use network devices, such as routers, switches, or hubs, to connect two or more computers together:

[![a network with a hub](https://study-ccna.com/wp-content/images/network_with_hub.jpg "a network with a hub")](https://study-ccna.com/wp-content/images/network_with_hub.jpg)

With the network topology above, all of the devices on the network can communicate with each other. That’s how computer networking works.

We’ll talk more about hubs and switches in just a moment. For now, remember that these devices serve as a central point for network connections to which all computers connect.

## Types of Computer Networks

Listed below are the most common types of computer networks:

- **[[Local Area Network]] ([[LAN]])** – LANs are commonly used in small to medium size companies, households, buildings, etc., with limited space.
- **[Personal Area Network] ([PAN])** – PAN covers a short distance of 10 meters. Bluetooth is an example of PAN.
- **[Metropolitan Area Network] ([MAN])** – MANs are used in a single geographic region, such as a city or town.
- **[Wide Area Network] ([WAN])** – WANs cover larger areas like different states and countries.
- **[Wireless Local Area Network] ([WLAN])** – Wireless LAN is used for wireless networks, connecting wired and wireless devices.
  
# TCP/IP vs OSI Model

There are two network models that are very much used nowadays. One is the OSI model, and the other is the TCP/IP model. TCP/IP vs. OSI is a persistent topic in the networking field, so let’s see how both models really differ.

## OSI Model

**OSI** (**Open System Interconnection**) model was created by the **International Organization for Standardization (ISO)**, an international standard-setting body. It was designed to be a reference model for describing the functions of a communication system.

The OSI model provides a framework for creating and implementing networking standards and devices and describes how network applications on different computers can communicate through the network media.

The OSI model has seven layers, each describing a different function of data traveling through a network. Here is the graphical representation of these layers:

[![TCP/IP vs OSI](https://study-ccna.com/wp-content/images/OSI_model.jpg "OSI model")](https://study-ccna.com/wp-content/images/OSI_model.jpg)

The layers are usually numbered from the last one, meaning that the Physical layer is considered the first layer. It is useful to remember these layers since there will certainly be some questions regarding them on the CCNA exam. Most people learn the mnemonic “**Please Do Not Throw Sausage Pizza Away**“:

[![OSI mnemonic](https://study-ccna.com/wp-content/images/OSI_mnemonic.jpg)](https://study-ccna.com/wp-content/images/OSI_mnemonic.jpg)

So, what is the purpose of these layers? They are most commonly used by vendors. They enable them to implement some functionality into a networking device, enabling easier interoperability with devices from other vendors.

Here is a brief description of each of the layers of the OSI model.

1. **Physical Layer** – defines how to move bits from one device to another. It details how cables, connectors, and network interface cards are supposed to work and how to send and receive bits.
2. **Data Link Layer** – encapsulates a packet in a frame. A frame contains a header and a trailer that enable devices to communicate. A header (most commonly) contains a source and destination MAC address. A trailer contains the Frame Check Sequence field, which detects transmission errors. The data link layer has two sublayers:
    - **Logical Link Control** – used for flow control and error detection.
    - **Media Access Control** – used for hardware addressing and controlling the access method.
3. **Network Layer** – defines device addressing, routing, and path determination. Device (logical) addressing is used to identify a host on a network (e.g. by its IP address).
4. **Transport Layer** – segments big chunks of data received from the upper layer protocols. Establishes and terminates connections between two computers. Used for flow control and data recovery.
5. **Session Layer** – defines establishing and terminating a session between the two systems.
6. **Presentation Layer** – defines data formats. Compression and encryption are defined at this layer.
7. **Application Layer** – this layer is the closest to the user. It enables network applications to communicate with other network applications.

It is a common practice to reference a protocol by the layer number or layer name. For example, HTTPS is referred to as an application (or Layer 7) protocol. Network devices are also sometimes described according to the OSI layer on which they operate – e.g. a Layer 2 switch or a Layer 7 firewall.

The following table shows which protocols reside on which layer of the OSI model:

[![OSI protocols](https://study-ccna.com/wp-content/images/OSI_protocols.jpg "OSI protocols")](https://study-ccna.com/wp-content/images/OSI_protocols.jpg)

## TCP/IP Model

The TCP/IP model was created in the 1970s by the **Defense Advance Research Project Agency (DARPA)** as an open, vendor-neutral, public networking model. Like the OSI model, it describes general guidelines for designing and implementing computer protocols. It consists of four layers: Network Access, Internet, Transport, and Application:

[![TCP IP model](https://study-ccna.com/wp-content/images/TCP_IP_model.jpg "TCP IP model")](https://study-ccna.com/wp-content/images/TCP_IP_model.jpg)

The following picture shows the comparison between the TCP/IP vs. OSI model:

[![TCP/IP vs OSI model layers comparison](https://study-ccna.com/wp-content/images/TCP_IP_and_OSI_model_comparison.jpg "TCP IP and OSI model comparison")](https://study-ccna.com/wp-content/images/TCP_IP_and_OSI_model_comparison.jpg)

As you can see from the picture above, the TCP/IP model has fewer layers than the OSI model. The OSI model’s Application, Presentation, and Session layers are merged into a single layer in the TCP/IP model. Also, the Physical and Data Link layers are called the Network Access layer in the TCP/IP model. Here is a brief description of each layer:

1. **Network Access Layer** – defines the protocols and hardware required to deliver data across a physical network.
2. **Internet Layer** – defines the protocols for logically transmitting packets over the network.
3. **Transport Layer** – defines protocols for setting up the level of transmission service for applications. This layer is responsible for the reliable transmission of data and the error-free delivery of packets.
4. **Application Layer** – defines protocols for node-to-node application communication and provides services to the application software running on a computer.

## Differences Between TCP/IP vs OSI Model

There are other differences between these two models besides the obvious difference in the number of layers. OSI model prescribes the steps needed to transfer data over a network, and it is very specific in it, defining which protocol is used at each layer and how. The TCP/IP model is not that specific. It can be said that the OSI model prescribes and TCP/IP model describes.