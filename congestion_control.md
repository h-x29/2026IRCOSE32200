\# TCP Congestion Control



Congestion control protects the network.



Congestion happens when routers, switches, or links in the middle of the network become overloaded.



\## Causes of Congestion



* Router queue overflow
* Switch queue overflow
* Saturated link capacity
* Too many packets being sent at once



\## Congestion Window



TCP uses a congestion window:



cwnd



The sender controls how much data can be sent based on the network condition.



\## Congestion Detection



TCP can detect or infer congestion from:



* Packet loss
* Triple duplicate ACKs
* Retransmission timeout
* Increased RTT
* ECN notification
* Example Algorithms
* Tahoe
* Reno
* CUBIC
* BBR



\## Key Idea



Flow control protects the receiver, while congestion control protects the network.

