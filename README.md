# Ethical Hacking Internship in Secure Dev Labs

Welcome to my portfolio repository documenting the practical security assessments, vulnerability research, and penetration testing tasks completed during my Ethical Hacking Internship at **Secure Dev Labs**.

This repository serves as a technical log of offensive security testing across web applications and network environments using industry-standard frameworks like **OWASP Top 10** and **PTES**.

---

## 🛠️ Tech Stack & Tools Covered
* **Operating System:** Kali Linux
* **Reconnaissance:** Subfinder, Amass, Nmap
* **Web Exploitation:** DVWA (Damn Vulnerable Web Application), Burp Suite
* **Automation & Exploitation:** SQLmap, Metasploit Framework (Meterpreter)

---

## 📌 Internship Roadmap & Tasks Breakdown

### 🔹 Task 1 & 2: Reconnaissance & Subdomain Enumeration
* **Objective:** Conduct passive and active discovery for asset attack surface mapping.
* **Actions Taken:** * Performed automated subdomain enumeration using tools like `Subfinder` and `Amass` against target bug bounty scopes on HackerOne.
  * Filtered live hosts and prepared reconnaissance structure logs for initial access mapping.

### 🔹 Task 3: Web Application Vulnerabilities (SQLi & XSS)
* **Objective:** Identify, exploit, and document critical application-layer vulnerabilities.
* **Actions Taken:**
  * **SQL Injection (SQLi):** Executed manual and automated Boolean-based, Error-based, and UNION-based SQLi scripts within a controlled DVWA laboratory.
  * **Database Dumping:** Utilized `SQLmap` for deep database schema enumeration, extracting structural tables, and validating data extraction hazards.
  * **Cross-Site Scripting (XSS):** Injected Reflected and Stored XSS payloads, analyzing application response actions, cookie tracking risks, and filter bypass methodologies via payload obfuscation.

### 🔹 Task 4: Infrastructure Auditing & Remote Code Execution (RCE)
* **Objective:** Perform full network penetration verification on vulnerable system components.
* **Actions Taken:**
  * **Service Fingerprinting:** Ran `Nmap` service scans to isolate an unprotected Java RMI registry listening on **TCP Port 1099** of a Metasploitable 2 environment.
  * **Exploitation:** Executed the `multi/misc/java_rmi_server` payload module in Metasploit to exploit the absence of a proper Java Security Manager.
  * **Post-Exploitation:** Established a stable reverse Meterpreter connection, verified full **ROOT** administrative privileges, and demonstrated system risk impact by accessing protected configurations.

---

## 🛡️ Executive Vulnerability Analysis (WH Architecture)

For each major exploit phase, findings were structurally isolated using the corporate reporting matrix:
* **What is the issue?** Comprehensive root cause definition of the configuration/injection flaw.
* **Where is the issue?** Exact mapping of target host endpoints, database rows, or network ports.
* **How to overcome the issue?** Actionable secure coding recommendations (such as Parameterized Queries, strict Context-Aware Output Encoding, Java Security Managers, and Host-Based Firewall/ACL controls).

---
