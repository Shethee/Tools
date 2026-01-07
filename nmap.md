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




















