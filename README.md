# Network Programming Snippets
These are the basic code snippets which I am learning to enhance my knowledge in network programming using python. Network programming is very important in respect of today's world. Network Programming is very important in new network

## Network Programming
Computer network programming involves writing computer programs that enable processes to communicate with each other across a computer network.

For connection-oriented communications, communication parties usually have different roles. One party is usually waiting for incoming connections; this party is usually referred to as "server". Another party is the one which initiates connection; this party is usually referred to as "client".

For connectionless communications, one party ("server") is usually waiting for an incoming packet, and another party ("client") is usually understood as the one which sends an unsolicited packet to "server". 

### Socket Buffer:

Recievers's socket buffer mean how much data can be in flight without acknowledgement. For a TCP/IP socket connection, the send and receive buffer sizes define the receive window. The receive window specifies the amount of data that can be sent and not received before the send is interrupted. If too much data is sent, it overruns the buffer and interrupts the transfer. The mechanism that control data transfer interruptions is referred to as flow control. If the receive window size for TCP/IP buffers is too small, the receive window buffer is frequently overrun, and the flow control mechanism stops the data transfer until the receive buffer is empty. The

The code for customizing the data buffer size implemented in python can be found <href>https://github.com/Cenrax/NetworkProgrammingSnippets/blob/master/ClientServer/Custom%20Buffer%20size.py</href>

**What is Socket? Do you know ?**

Stream sockets allow processes to communicate using TCP. A stream socket provides bidirectional, reliable, sequenced, and unduplicated flow of data with no record boundaries. After the connection has been established, data can be read from and written to these sockets as a byte stream. The socket type is SOCK_STREAM.

Datagram sockets allow processes to use UDP to communicate. A datagrm socket supports bidirectional flow of messages. A process on a datagram socket can receive messages in a different order from the sending sequence and can receive duplicate messages. Record boundaries in the data are preserved. The socket type is SOCK_DGRAM.

Raw sockets provide access to ICMP. These sockets are normally datagram oriented, although their exact characteristics are dependent on the interface provided by the protocol. Raw sockets are not for most applications. They are provided to support developing new communication protocols or for access to more esoteric facilities of an existing protocol. Only superuser processes can use raw sockets. The socket type is SOCK_RAW

***Innovation areas in socket***
With the advancement of technology and with the embedding of SDN and IP Addresses innovation in socket is highly required in my opinion. Can we thing of a intelligent socket? A socket is smart

