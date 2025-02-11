# Cyber Attack Report: MS2 21 Coded Backdoor (using Metasploit too)

## 1. Overview
- **Attack Name:** [vsftpd 2.3.4 Backdoor Command Execution]
- **Date of Attack:** [2025-02-02]
- **Targeted System:** [MS2 Server]
- **Attack Type:** [RCE, Phishing, SQL Injection, etc.]
- **Impact:** [Data breach, system compromise, financial loss, etc.]

## 2. Attack Methodology
### 2.1 Initial Access
- Ran Natdiscover.
- Ran Nmap on discovered servers.
- Found server with known backdoor for MS2 on FTP.

### 2.2 Execution 1
- Telnet on port 21.
- Add backdoor code to USER and dummy PASS.
- Close 21, telnet to backdoor.
- Root access confirmed, ftp server breached.

### Execution 2
- Opened Metasploit Framework.
- Searched for vsftpd.
- Configured payload, configured RHOST.
- Ran and gained root access.

### 2.3 Persistence
- 

### 2.4 Lateral Movement
- How the attack spread within the network.

### 2.5 Exfiltration
- What data was stolen, and how.

## 3. Indicators of Compromise (IoCs)
- **IP Addresses:** See `indicators_of_compromise/ips.txt`
- **Malicious Domains:** See `indicators_of_compromise/domains.txt`
- **File Hashes:** See `indicators_of_compromise/hashes.txt`

## 4. Logs and Analysis
- Log files available in the `logs/` directory.
- Analysis of suspicious activities in logs.

## 5. Mitigation and Remediation
- Patch details and remediation steps in `mitigations/`.

## 6. Proof of Concept (PoC)
- If applicable, a recreated PoC exploit is in `exploits/`.

## 7. References
- CVE Details: See `references/CVE_details.md`
- Articles: See `references/articles.md`
