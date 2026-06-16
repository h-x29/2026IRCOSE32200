\# Reliable and In-Order Delivery



TCP guarantees reliable and in-order delivery.



\## Sequence Number



TCP uses sequence numbers to track bytes in the TCP byte stream.



The sequence number represents the first byte of the segment.



Example:



If a segment carries bytes 1000 to 1999, then:



```text

Sequence Number = 1000



\## ACK Number



The ACK number means the next byte the receiver expects.



Example:



ACK = 2000



This means:



The receiver has successfully received all bytes up to 1999.

The next expected byte is 2000.

Retransmission



If the sender does not receive an ACK in time, TCP assumes the segment may be lost and retransmits it.



\## Key Idea



TCP reliability is achieved using sequence numbers, ACK numbers, timers, and retransmission.

