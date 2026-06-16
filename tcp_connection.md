\# TCP Connection-Oriented Communication



TCP is a connection-oriented protocol.



Before data can be exchanged, the client and server must establish a connection.



\## Common TCP Socket States



\### LISTEN



The server socket is waiting for client connection requests.



\### ESTABLISHED



The connection has been successfully established.

Data delivery is now possible.



\### CLOSING



The connection is being terminated.



\## Why Connection State Matters



TCP sockets have states because TCP needs to manage the full lifetime of a connection.



This includes:



* Connection establishment
* Data transmission
* Reliable delivery
* Connection termination



\## Key Idea



Unlike UDP, TCP must connect first before sending normal data.

