# TryHackMe - RootMe Penetration Testing Report

## Objective

--------------
## Scope
 - Platform: TryHackMe
 - Room: RootMe
 - Target: Virtual Machine

 --------

 ## Methodology
 1. Reconnaissance
 2. Enumeration
 3. Initial Acess
 4. Privilege Escalation
 5. Post Exploitation
 
 --------

 # Phase 1 - Reconnaissance
 ## Objective 
 The objective of this assessment was to identify open ports, running services, and potential attack vectors on the target machine.
 ## Nmap Scan
 **Command**
 ```bash
nmap -Pn -sC -sV -p- <TARGET_IP> -oN nmap_rootme.txt
```
![Nmap Results](screenshots/nmap_rootme.png)

### Results

The nmap scan identified two open TCP ports:
| Port   | Service  | Version            |
|--------|----------|--------------------|
| 22     | SSH      | OpenSSH            |
|80      | HTTP     | Apache httpd 2.4.42|

### Analysis
The target exposes an SSH service on port 22 and a web sever on port 80. Since SSH requires valid credentials, the web server presents the most promising initial attack surface. The next phase will focus on enumerating the web application to identify hidden directories, files, and potential vulnerabilities.




 # Phase 2 - Enumeration



 # Phase 3 - Initial Access


 # Phase 4 - Privilege Escalation

----------
 # Tools Used
  - Nmap
  - Gobuster / FFUF
  - Netcat
  - Bash
  - GTOBins

  -----------

  # Recommendations

  
 
