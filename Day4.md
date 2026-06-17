Day4 - Tcp vs Udp,Portscanning,Threeway handshake and wireshark practice

1.TCP(Transmission Control Protocol-
It is a communicaton protocol that guarantees delivery of data between to devices.

Reliable
Slow(Because it check everything)
Usedfor(Website,email,filedownloads and banking)
Example ports(80HTTP, 443HTTPS AND 23SSH)

Three way handshake of TCP

First step-The sender computer send the S-Y-N (Synchronise) message to receiver computer.
Second Step-The Receiver computer will respond with S-Y-N ACK responding the message send by the first computer or sender.
Third Step-Then after S-Y-N ACK message is received by the sender the sender computer send the ACK received message to the receive computer.

Once this done,finally data can be delivered.

2.UDP(User Datagram Protocol)
This protocol is connection less which means it doesn’t establish session and doesn’t guarante the data delivery.

Unreliable(It doesn’t check if data received or not)
Faster(Because it doesn’t check)
Used for(gaming.video call and live streaming)
Example ports(53Dns,123NTP)

3.Port and Portscanning
Port are the virtual meeting point or logical connection that are used by program or services to exchange data.

Portscanning is a technique hacker used to discover the backdoor that program or services used exchsnge data so they can find vulnerbility.

4. What is a SYN flood attack?
It is Ddos type of hacking when a hacker send a SYN packets while spoofing his ip address,num of SYN packets are send and server try to Send SYN Ack message but they never get the AcK message which leave the ports open They send numerous SYN packets get SYN ACK message which leave the ports open that drains the memeory of server.



YOUR DAY 4 NOTES — Write These in Your Own Words
Answer each question in your own words like you did for Days 1, 2 and 3:
•	What is TCP?
•	What is UDP?
•	What is the difference between TCP and UDP?
•	What are the 3 steps of the handshake?
•	What is a SYN flood attack?
•	What is port scanning?
•	What did you see in Wireshark when you filtered by tcp?
