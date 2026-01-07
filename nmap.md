Nmap(network mapper) is a open source tool used for network discovery and security auditing. it also assists in the exloration of network hosts and services providing information about open ports, operating system and other details.

Address Resolution Protocol (ARP) is responsible for finding the MAC (hardware) address related to a specific IP address. It works by broadcasting an ARP query, "Who has this IP address? Tell me." And the response is of the form, "The IP address is at this MAC address."
. ARP scan: This scan uses ARP requests to discover live hosts
. ICMP scan: This scan uses ICMP requests to identify live hosts

Transmission Control Protocol (TCP) is a connection-oriented protocol requiring a TCP three-way-handshake to establish a connection. TCP provides reliable data transfer, flow control and congestion control. Higher-level protocols such as HTTP, POP3, IMAP and SMTP use TCP

User Datagram Protocol (UDP) is a connectionless protocol; UDP does not require a connection to be established. UDP is suitable for protocols that rely on fast queries, such as DNS, and for protocols that prioritise real-time communications, such as audio/video conferencing and broadcast.
. TCP/UDP ping scan: This scan sends packets to TCP ports and UDP ports to determine live hosts.

NMAP:
1. Enumerate targets
2. Discover Live hosts
3. Reverse-DNS lookup
4. Scan ports
5. Detect versions
6. Detect os
7. Traceroute
8. Scripts
9. Write output

### Nmap Host Discovery
1. Subnetworks
2. Enumering Targets
3. Discovering Live Hosts
4. Nmap Host discovery using ARP
5. Nmap Host discovery Using ICMP
6. Nmap Host using TCP and UDP
7. Using reverse dns lookup

### Nmap basic Port Scanning
1.TCP and UDP Ports
2. TCP flags
URG: Urgent flag indicates that the urgent pointer filed is significant. The urgent pointer indicates that the incoming data is urgent, and that a TCP segment with the URG flag set is processed immediately without consideration of having to wait on previously sent TCP segments.
ACK: Acknowledgement flag indicates that the acknowledgement number is significant. It is used to acknowledge the receipt of a TCP segment.
PSH: Push flag asking TCP to pass the data to the application promptly.
RST: Reset flag is used to reset the connection. Another device, such as a firewall, might send it to tear a TCP connection. This flag is also used when data is sent to a host and there is no service on the receiving end to answer.
SYN: Synchronize flag is used to initiate a TCP 3-way handshake and synchronize sequence numbers with the other host. The sequence number should be set randomly during TCP connection establishment.
FIN: The sender has no more data to send.
3. TCP connect Scan
4. TCP syn Scan
5. UDP scan
6. Fine-Tuning Scope and Performance
7. Idle/Zombie Scan

### Nmap Advanced Port Scans
1. TCP null scan, FIN scan and Xmas Scan
1.1 Null Scan
1.2 FIN Scan
1.3 Xmas Scan
2. TCP top maimon scan
3. TCP ack, window and custom scan
4. Spoofing and Decoy
5. fragmented packets


### Nmap Post Port scan
1. Service detection
2. Os detection and Traceroute
3. Nmap Scripting Engine(NSE)
4. Savings the output





### study about:
1. TCP packet
2. TCP ping
3. TCP handshake
4. UDP Packet
5. ARP packet
6. Ping Packet
7. Overall types of packets.
8. ports and protocols
9. local network and internetwork
10. HTTP
11. DNS
12. SSH, open ssh
13. Flags and tickets
14. TCP flags
15. TCP 3way handshake
16. If the TCP segment has a size of 64, and -ff option is being used, how many IP fragments will you get?



## NMAP commands
1. -sS ( for Syn Scan)
2. -sU( for UDP scan)
3. -O (OS scan)
4. -sL stands for Scan List in nmap. It is used to list the targets without actually sending them any packets to them.
   It helps in identifying live hosts without performing a scan.
5. sudo nmap -PR -sn machine_ip/24 is used to discover live systems on the same subnet as the specified target machine. The "PR" option tells nmap to perform an arp scan which is effective in local 
6. -PP
7. -PM
8. -PE
9. 




















