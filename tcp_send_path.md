\# TCP Send Path in Linux



When a user program sends data using a TCP socket, the data passes through several kernel functions.



\## Main TCP Output Functions



tcp\_sendmsg()

tcp\_write\_xmit()

tcp\_transmit\_skb()



\# Step 1: tcp\_sendmsg()



This function copies user data from user space into kernel space.



It also creates socket buffers called sk\_buff.



Main tasks:



* Copy payload from user space
* Create sk\_buff buffers
* Put buffers into the write queue



\# Step 2: tcp\_write\_xmit()



This function checks whether the data is allowed to be sent.



It considers:



* Flow control
* Congestion control
* Receiver window
* Congestion window



If sending is not allowed, the data remains in the queue.



\# Step 3: tcp\_transmit\_skb()



This function prepares the packet for transmission.



Main tasks:



* Build TCP header
* Calculate checksum
* Handle TCP options
* Pass packet to IP layer



\## Simplified Flow



write()

\-> sock\_sendmsg()

\-> inet\_sendmsg()

\-> tcp\_sendmsg()

\-> tcp\_write\_xmit()

\-> tcp\_transmit\_skb()

\-> ip\_queue\_xmit()



\## Key Idea



TCP does not immediately send all written data.

It checks reliability, flow control, and congestion control before transmission.

