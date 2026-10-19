# Task 2: Network Security & Scanning

A complete hands-on demonstration of network reconnaissance, port scanning, vulnerability management, packet analysis, and firewall configuration carried out on target test environments (e.g., Metasploitable2).

---

## 📌 Project Overview
This repository contains the detailed methodology, technical findings, and scan artifacts for **Task 2 (Network Security & Scanning)** of the Cybersecurity & Ethical Hacking Internship Program.

The primary objective is to gain practical experience in identifying live hosts, discovering open services, assessing system vulnerabilities, analyzing unencrypted network traffic, and configuring defensive firewall rules.

---

## 🛠️ Tools & Technologies Used
* **Reconnaissance:** `Whois`, `Nslookup`, Google Dorking, Shodan, Ping Sweep
* **Port & Service Scanning:** Nmap (`-sS`, `-sU`, `-sV`, `-O`)
* **Vulnerability Scanning:** OpenVAS / Nessus Essentials
* **Packet Analysis:** Wireshark, `hping3`
* **Firewall Configuration:** Linux `iptables`

---

## 🚀 Work Completed & Modules

### 1. Reconnaissance
* **Passive Recon:** Executed OSINT techniques using `Whois`, `Nslookup`, Google Dorks, and Shodan to gather public network information.
* **Active Recon:** Performed ICMP ping sweeps and service banner grabbing to enumerate target assets.

### 2. Port & Service Scanning
* Executed TCP SYN (`-sS`) and UDP (`-sU`) stealth scans using Nmap.
* Enumerated running services (`-sV`) and target operating systems (`-O`) on the Metasploitable2 VM.

### 3. Vulnerability Scanning
* Deployed OpenVAS / Nessus Essentials to perform a full system scan.
* Analyzed vulnerability findings categorized by severity (**Critical**, **High**, **Medium**, **Low**).

### 4. Packet Analysis with Wireshark
* Captured and filtered raw HTTP, FTP, and DNS network packets.
* Extracted plaintext user credentials from unencrypted FTP traffic.
* Simulated a SYN flood attack using `hping3` and analyzed packet patterns.

### 5. Firewall Configuration
* Configured custom `iptables` rules to allow/deny specific port traffic.
* Demonstrated active defense by blocking port scanning attempts in real-time.

---


