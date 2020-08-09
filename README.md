# NetworkProgrammingSnippets
These are the basic code snippets which I am learning to enhance my knowledge in network programming using python. Network programming is very important in respect of today's world.

## Network Programming
Computer network programming involves writing computer programs that enable processes to communicate with each other across a computer network.

For connection-oriented communications, communication parties usually have different roles. One party is usually waiting for incoming connections; this party is usually referred to as "server". Another party is the one which initiates connection; this party is usually referred to as "client".

For connectionless communications, one party ("server") is usually waiting for an incoming packet, and another party ("client") is usually understood as the one which sends an unsolicited packet to "server". 

### Socket Buffer:

Recievers's socket buffer mean how much data can be in flight without acknowledgement. For a TCP/IP socket connection, the send and receive buffer sizes define the receive window. The receive window specifies the amount of data that can be sent and not received before the send is interrupted. If too much data is sent, it overruns the buffer and interrupts the transfer. The mechanism that controls data transfer interruptions is referred to as flow control. If the receive window size for TCP/IP buffers is too small, the receive window buffer is frequently overrun, and the flow control mechanism stops the data transfer until the receive buffer is empty.

The code for customizing the data buffer size implemented in python can be found <href>https://github.com/Cenrax/NetworkProgrammingSnippets/blob/master/ClientServer/Custom%20Buffer%20size.py</href>
