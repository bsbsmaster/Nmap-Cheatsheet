# Nmap-Cheatsheet
Nmap-Cheatsheet
Category	Command	Description
Basic Scanning		
nmap [target]	Scan target
nmap -p [port(s)] [target]	Scan specific port(s)
nmap -F [target]	Fast scan (top 100 ports)
nmap -p- [target]	Scan all ports
Host Discovery		
nmap -sn [target]	Disable port scan (Ping Scan)
nmap -Pn [target]	Disable ICMP Echo Requests
nmap -n [target]	Disable DNS Resolution
TCP Scan Types		
nmap -sS [target]	TCP SYN Scan
nmap -sA [target]	TCP ACK Scan
nmap -sF [target]	TCP FIN Scan
nmap -sX [target]	TCP Xmas Scan
nmap -sN [target]	TCP Null Scan
UDP Scan		
nmap -sU [target]	UDP Scan
Service Version Detection		
nmap -sV [target]	Version Detection
Script Scanning		
nmap -sC [target]	Script Scan (default scripts)
nmap --script [script] [target]	Specify script
Operating System Detection		
nmap -O [target]	OS Detection
Output Options		
nmap -oA [filename] [target]	Output to all formats
nmap -oN [filename] [target]	Normal output to file
nmap -oG [filename] [target]	Grepable output to file
nmap -oX [filename] [target]	XML output to file
Performance Options		
nmap --max-retries [num] [target]	Number of retries
nmap --stats-every=[time] [target]	Display status interval
nmap -v / -vv [target]	Verbose output
nmap --initial-rtt-timeout [time] [target]	Initial RTT timeout
nmap --max-rtt-timeout [time] [target]	Maximum RTT timeout
nmap --min-rate [rate] [target]	Minimum packet rate
nmap -T [0-5] [target]	Timing template
Firewall Evasion Techniques		
nmap -f [target]	Fragment packets
nmap --mtu [value] [target]	Set MTU value
nmap --data-length [value] [target]	Set packet data length
nmap --ip-options [value] [target]	Set IP options
Spoofing Options		
nmap -S [spoofed_ip] [target]	Spoof source IP address
nmap -g [portnum] [target]	Source port
DNS Options		
nmap --dns-servers [server] [target]	Use specific DNS server
nmap --system-dns [target]	Use system's DNS server
Additional Techniques		
nmap --script-updatedb	Update Nmap script database
nmap --traceroute [target]	Perform traceroute
nmap --badsum [target]	Generate packets with bad checksums
