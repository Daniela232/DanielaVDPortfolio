> **Looking for the pink portfolio page?** [View the styled website version](https://daniela232.github.io/DanielaVDPortfolio/cybersecurity-projects.html). This Markdown file is the GitHub source document.

# CodePath Cybersecurity Project Showcase

This page documents selected hands-on cybersecurity work from CodePath CYB101 and CYB102. The descriptions are based on my course submission write-ups. All work was conducted in educational, simulated, or authorized lab environments. This page intentionally excludes student records, credentials, original malicious payloads, and private Google Docs submissions.

## Security Monitoring and Incident Investigation

### SIEM Malware Investigation — Splunk (CYB102 Project 5)
**Tools:** Splunk, SPL, log analysis

- Investigated a simulated malware upload involving `EvilScript.exe` in the PathCode environment.
- Used SPL queries across security event data to identify the source IP, suspicious upload activity, and browser user-agent.
- Compared the malicious upload with another file upload to distinguish suspicious activity from benign activity.
- Documented searches and answers for all 15 assigned CTF questions.

**Sample investigation query:**
```spl
index=pathcode "3AADBF7E527FC1A050E1C97FEA1CBA4D"
```

### Malware Incident Response — Catalyst and VirusTotal (CYB102 Project 6)
**Tools:** Catalyst, Splunk, VirusTotal, NIST incident response concepts

- Documented a simulated malware incident involving repeated login attempts and the upload of `EvilScript.exe`.
- Recorded a file hash, investigated security-log evidence, and summarized detection and response gaps.
- Recommended stronger MFA, file-upload monitoring, endpoint protection, and access controls.
- Wrote a NIST incident response framework analysis covering preparation, detection, containment, recovery, and lessons learned.

### IOC Correlation and Monitoring — Splunk (CYB102 Project 7)
**Tools:** Splunk, SPL, VirusTotal, threat intelligence

- Correlated threat-intelligence IP addresses with simulated network proxy logs.
- Documented two matches, including timestamps and affected workstation names.
- Wrote an SPL search for a threat-intelligence monitoring dashboard.
- Evaluated why reputation data must be interpreted in its historical context.

### Phishing / Business Email Compromise Investigation — Wireshark (CYB102 Project 1)
**Tools:** Wireshark, SMTP, PCAP analysis

- Examined packet-capture files to identify suspicious email activity and isolate relevant traffic.
- Applied `smtp` and `smtp.data.fragment` display filters.
- Identified a suspicious source IP and documented three phishing email subject lines.

### File Integrity Monitoring and Attack Attribution — Linux Audit (CYB102 Project 2)
**Tools:** Linux auditd, audit logs

- Investigated simulated changes to protected files.
- Identified four affected files and matched them to three separate attack scripts.
- Documented the correspondence between the observed file modifications and the attack source.

## Network Defense and Security Testing

### Application-Layer DoS Mitigation — nginx (CYB102 Project 4)
**Tools:** nginx, Wireshark, network monitoring, Slowloris lab

- Evaluated a controlled Slowloris denial-of-service simulation against a lab web server.
- Documented nginx mitigation configuration and compared connection behavior before and after defensive changes.
- Analyzed packet captures with Wireshark TCP Conversations and TCP flags to distinguish vulnerable and mitigated server behavior.

### FTP Service Exploitation — Controlled Metasploitable Lab (CYB101 Project 4)
**Tools:** Kali Linux, Nmap, Metasploit

- Used Nmap to examine a deliberately vulnerable FTP service on port 21.
- Executed a course-authorized Metasploit lab exploit and verified access through the resulting shell.
- Received full required-project credit (20/20) in the submission rubric.

## Digital Forensics and Security Fundamentals

### Image Steganography and Metadata — Steghide (CYB101 Project 6)
**Tools:** Steghide, ExifTool, Linux

- Investigated hidden information within image files using steganography techniques.
- Documented commands for inspecting, extracting, and reading concealed data.
- Received full required-project credit (20/20) in the submission rubric.

### Cryptography and Reconnaissance CTF — CyberChef (CYB101 Project 1)
**Tools:** CyberChef, Base64, rotation ciphers, file analysis

- Solved and documented seven of the course's cryptography, reconnaissance, and security-fundamentals challenges.
- Used CyberChef to decode a Base64 message and a rotation cipher, and recovered a flag through file-format investigation.
- Received 16/16 points on the required-project rubric.

### Payload Construction and Detection Concepts — MSFvenom (CYB101 Project 5)
**Tools:** MSFvenom, isolated Linux lab

- Constructed three controlled training payload files: a message-box demonstration, a multi-payload demonstration, and an encoder-based demonstration.
- Documented terminal commands and outputs for the three required payload-creation steps.
- Received 18/20 points; VirusTotal stretch challenges were not credited.
- No payload executables or deployable malware samples are included in this repository.

## Other coursework

Additional classroom work includes password-hash auditing with John the Ripper, host reconnaissance with Shodan, and directory-traversal demonstrations. Detailed technical claims about optional challenges are omitted when the submission evidence does not establish their completion.

## Security and publication notes

These are **educational labs**, not production penetration tests or investigations of real employers. Original course handouts, private submissions, raw malicious samples, secrets, and third-party data are not redistributed. Findings are summarized in original language for a public professional portfolio.
