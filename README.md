# Analyze-Network-Layer-Communication
Exemplar
Cybersecurity Incident Report: Network Traffic Analysis

Issue with DNS and ICMP traffic.

It looks like the DNS server is having problems because the UDP protocol shows it's down. The network analysis also caught an error in the ICMP echo reply, saying "udp port 53 unreachable." Since Port 53 is crucial for DNS, it suggests the DNS server is likely not responding.

What happened and why.

Today at 1:23 p.m., customers told us they couldn't access the website and got a "destination port unreachable" message. Our IT team is on it. We used tcpdump to check the network and found that DNS port 53 wasn't reachable. Now we're figuring out if the DNS server is down or if the firewall is blocking traffic to port 53. It could be because of an attack or a mistake in the settings
