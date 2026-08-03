# Cybersecurity-Home-Lab
A virtual cybersecurity lab demonstrating vulnerability assessment and penetration testing using Kali Linux and Metasploitabl
# Cybersecurity Home Lab - Vulnerability Assessment & Penetration Testing

## Overview

This project demonstrates a controlled penetration testing environment built using VirtualBox. 

The objective was to simulate an enterprise server security assessment by identifying vulnerabilities, scanning services, and performing ethical exploitation against an intentionally vulnerable machine.

## Lab Environment

### Attacker Machine
- Kali Linux
- Tools:
  - Nmap
  - Nikto
  - Metasploit Framework

### Target Machine
- Metasploitable 2
- Ubuntu-based vulnerable server
- Purpose: Security testing practice

## Network Configuration

VirtualBox Host-Only Network:

Kali Linux:
192.168.56.100

Metasploitable 2:
192.168.56.103


## Testing Methodology

### 1. Network Discovery

Used Nmap to identify:

- Open ports
- Running services
- Service versions

Command:

nmap -sV 192.168.56.103


### 2. Web Vulnerability Assessment

Used Nikto to identify:

- Outdated web server software
- Missing security headers
- Exposed directories


### 3. Exploitation Testing

Used Metasploit Framework to demonstrate exploitation of:

VSFTPD 2.3.4 Backdoor Vulnerability

CVE:
CVE-2011-2523


## Results

Identified vulnerabilities including:

- Outdated Apache server
- Outdated PHP version
- Directory indexing
- Vulnerable FTP service


## Tools Used

| Tool | Purpose |
|---|---|
| Kali Linux | Penetration testing platform |
| VirtualBox | Virtual lab environment |
| Nmap | Network scanning |
| Nikto | Web vulnerability scanning |
| Metasploit | Exploitation framework |


## Disclaimer

This project was performed in an isolated home lab environment for educational purposes only.
