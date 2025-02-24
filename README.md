# nmap

nmap scanning options 


Basic Network Scan:
Scan the entire subnet to discover live hosts:
nmap -sn 192.168.1.0/24


Full Port Scan (TCP) on All Live Hosts:
Identify all open TCP ports on the network:
nmap -p- 192.168.1.0/24


Service & Version Detection:
See what services are running and their versions:
nmap -sV -sC 192.168.1.0/24


Scan for Vulnerabilities (with Scripts):
Use Nmap Scripting Engine (NSE) for vulnerability detection:
nmap -sV --script vuln 192.168.1.0/24


Detect Firewall and IDS/IPS Rules:
Identify network security devices and their configurations:
nmap -sA 192.168.1.0/24


Scan for SSL/TLS Misconfigurations:
Check for outdated or weak SSL/TLS protocols:
nmap --script ssl-enum-ciphers -p 443 192.168.1.0/24


PCI DSS Compliance Scan:
If you want to specifically check for PCI-related vulnerabilities:
nmap --script pci-dss 192.168.1.0/24
