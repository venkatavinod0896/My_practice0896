Module 2 - Computer Network

Lab 1: Test Connectivity
Tasks:
Ping your gateway and observe TTL value.


Ping a public server like 8.8.8.8 (Google DNS).


Ping a domain name (e.g., google.com) — does DNS resolution work?
 Commands Hint:
 ping <ip>, ping <domain>

Lab 2: Essential Networking Commands
Objective: Use diagnostic tools.
 Tasks:
Display your network interfaces with ifconfig or ip a.


Trace the route to google.com using traceroute.


Show ARP table and analyze entries.


Examine the routing table using route -n.
 Commands: ifconfig, traceroute, arp -n, route -n, ip route
Lab 3: DNS and Name Resolution
Objective: Investigate how DNS works.
 Tasks:
Use nslookup or dig to resolve www.github.com.


Identify the IP address of your DNS server.


Flush and recheck DNS cache.


Explain difference between recursive and iterative DNS queries.
 Commands: dig, nslookup, cat /etc/resolv.conf

Lab 4: Use Traceroute
Tasks:
Run a traceroute to google.com.


How many hops are there?


Identify which hop belongs to your ISP.
 Commands Hint:
 traceroute google.com
 (On Windows: tracert google.com)
Lab 5: Check Host Reachability with telnet/nc
Tasks:
Check if port 80 on a server is reachable.


Check SSH port 22 connectivity.


Test a closed port and observe behavior.
 Commands Hint:
 telnet <ip> <port> or nc -zv <ip> <port>
Lab 6: Default Gateway & Routing Table
Tasks:
Display your routing table.


Add a temporary static route to another network.


Delete that static route.
 Commands Hint:
 ip route show,
 ip route add,
 ip route del
Lab 7: Network Security and Attack Simulation
Objective: Identify and defend against common attacks.
 Tasks:
Simulate a simple ping flood using ping -f (in a safe, local test).


Use netstat to detect unusual open connections.


Discuss mitigation techniques for DDoS and Man-in-the-Middle attacks.


Identify open ports and services using nmap.
 Commands: ping, netstat -tulnp, nmap -sS localhost
Lab 8: Hosts File Resolution Priority
Tasks:
Add a fake entry for facebook.com in /etc/hosts.


Curl to see if it resolves to your fake IP.


Remove the entry and test again.
Lab 9: Understand Ports, Services & Firewall Rules
Tasks:
List which services are listening on your machine.


Identify which ports are open for TCP and UDP.


Enable or disable a port using ufw (Ubuntu firewall).


Verify whether a port is reachable using nc or telnet.
Lab 11: HTTP Requests & Web Debugging
Tasks:
Use curl to fetch the homepage of a website (e.g., example.com).


View only HTTP response headers.


Send a HEAD request to check server details.


Test an HTTPS endpoint and observe certificate details
