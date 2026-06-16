\# COSE322 System Programming Optional Project



\## Student Information

* Name: 이휘싱
* Course: COSE322 System Programming
* Topic: Lecture 11 - TCP in Linux



\## Repository Purpose



This repository is created for the COSE322 System Programming optional project.



The content is based on my personal study notes for Lecture 11: TCP in Linux. It summarizes important TCP concepts and includes simple TCP client/server practice code.



\## Content



* TCP overview
* TCP connection-oriented communication
* Reliable and in-order delivery
* Selective ACK
* Flow Control
* Congestion Control
* Linux TCP data structures
* TCP send path
* TCP receive path
* Simple TCP client/server examples



\## Learning Reflection



Through studying TCP in Linux, I learned how the Linux kernel implements reliable communication using sequence numbers, acknowledgments, retransmissions, flow control, and congestion control.



I also learned about important TCP-related kernel data structures such as:



* struct socket
* struct sock
* struct tcp\_sock
* struct sk\_buff
* struct tcphdr



The most interesting topic was understanding how Linux decides when packets can be transmitted through flow control and congestion control mechanisms.



This repository serves as my personal study notes for Lecture 11.

