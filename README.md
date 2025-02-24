# nmap

nmap scanning options 


Basic Network Scan:</br>
Scan the entire subnet to discover live hosts:</br>
nmap -sn 192.168.1.0/24</br>


Full Port Scan (TCP) on All Live Hosts:</br>
Identify all open TCP ports on the network:</br>
nmap -p- 192.168.1.0/24</br>


Service & Version Detection:</br>
See what services are running and their versions:</br>
nmap -sV -sC 192.168.1.0/24</br>


Scan for Vulnerabilities (with Scripts):</br>
Use Nmap Scripting Engine (NSE) for vulnerability detection:</br>
nmap -sV --script vuln 192.168.1.0/24</br>


Detect Firewall and IDS/IPS Rules:</br>
Identify network security devices and their configurations:</br>
nmap -sA 192.168.1.0/24</br>


Scan for SSL/TLS Misconfigurations:</br>
Check for outdated or weak SSL/TLS protocols:</br>
nmap --script ssl-enum-ciphers -p 443 192.168.1.0/24</br>


PCI DSS Compliance Scan:</br>
If you want to specifically check for PCI-related vulnerabilities:</br>
nmap --script pci-dss 192.168.1.0/24</br>
