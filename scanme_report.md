<img width="951" height="412" alt="image" src="https://github.com/user-attachments/assets/8d4ed709-c903-4184-8364-21800b3b4f3e" /># Task 2 — Network Security & Scanning

## Objective
Learn reconnaissance, scanning, and network traffic analysis techniques against the lab target.

## 1. Reconnaissance
Performed passive recon (Whois, Nslookup, Google Dorking, Shodan) and active recon (ping sweep, banner grabbing) against the lab target to gather host and service information before scanning.

Screenshots: 
nslookup_whois output: ![Kali Terminal](scan_me/VirtualBox_kali_nslookup_whois.png) 
Google Dork Results: ![Kali Terminal](scanme/VirtualBox_kali_googledork.png)
Shodan Search Result: ![Kali Terminal](scanme/setup/VirtualBox_kali_shodan.png)
active recon Output: ![Kali Terminal](scanme/setup/VirtualBox_kali_activerecon2.png)

## 2. Port & Service Scanning
Ran Nmap TCP (-sS) and UDP (-sU) scans against Metasploitable2, followed by service version detection (-sV) and OS detection (-O) to build a full picture of open ports and running services.

Screenshots: /screenshots/scanning
Nmap TCP Scan: ![Kali Terminal](scanme/setup/VirtualBox_kali_TCPSCAN.png)
Nmap UDP Scan: ![Kali Terminal](scanme/setup/VirtualBox_kali_UDPSCAN.png)
Nmap Service Version Detection: ![Kali Terminal](scanme/setup/VirtualBox_kali__PORT_SERVICE_VERSION_OS.png)
Nmap OS Detection: ![Kali Terminal](scanme/setup/VirtualBox_kali__OSFINGERPRINTING.png)

## 3. Vulnerability Scanning
Set up OpenVAS and scanned the Metasploitable2 VM, then analyzed the resulting report by severity (Critical/High/Medium/Low).

Screenshots: /screenshots/vuln-scan
OpenVAS Setup
Vulnerability Scan Report

## 4. Packet Analysis with Wireshark
Captured HTTP, FTP, and DNS traffic on the lab network, filtered out credentials from unencrypted FTP traffic, and analyzed a simulated SYN flood attack generated with hping3.

Screenshots: /screenshots/packet-analysis
HTTP/FTP/DNS Capture
FTP Credentials Filter
SYN Flood Analysis

## 5. Firewall Basics
Created iptables rules to allow/deny specific ports, then demonstrated blocking an active port scan attempt.

Screenshots: /screenshots/firewall
Iptables Rules
Blocked Port Scan
