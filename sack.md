\# SACK: Selective Acknowledgment



SACK means Selective ACK.



It allows the receiver to acknowledge non-continuous blocks of data.



\## Without SACK



If byte 2 is lost but bytes 3, 4, and 5 arrive, the receiver can only report that byte 2 is still expected.



The sender may think later bytes were also lost.



\## With SACK



The receiver can say:



Byte 2 is missing, but bytes 3, 4, and 5 were received.



Then the sender only retransmits the missing byte.



&#x20;## Advantage



SACK improves efficiency because TCP does not need to retransmit data that was already received.



\## Key Idea



SACK helps TCP recover from packet loss more efficiently.

