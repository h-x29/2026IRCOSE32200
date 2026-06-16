\# TCP Flow Control



Flow control protects the receiver.



The receiver has a limited buffer size, so the sender should not send more data than the receiver can handle.



\## Receive Window



The receiver advertises its available buffer space using the receive window.



This is called:



rwnd



Example:



rwnd = 5000



This means the receiver can currently accept 5000 more bytes.



\## Why Flow Control Is Needed



Each TCP socket has a finite receive buffer.



If the sender sends too much data too quickly, the receiver buffer may overflow.



\## Adjustable Buffer Size



The receive buffer size can be adjusted using settings such as:



setsockopt(SO\_RCVBUF)



or Linux system settings such as:



net.ipv4.tcp\_rmem



\## Key Idea



Flow control prevents receiver-side buffer overflow.

