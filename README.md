# Blue-Team-Cyber-Threat-Analysis-SPLUNK-Investigation-with-Boss-of-the-SOC-v3-Dataset

As a Blue Team member, I conducted a cyber threat investigation using the Boss of the SOC v3 dataset and SPLUNK, mapping adversary actions to the Cyber Kill Chain and MITRE ATT&amp;CK frameworks.

Key Findings:

* Brute Force & Password Spraying: Attackers attempted unauthorized access from IP addresses based in the Netherlands.
* Phishing & Credential Harvesting: Macro-enabled malware (W97M.Empstage) was delivered through email.
* Exposed AWS Credentials: Leaked AWS keys allowed for privilege escalation.
* Malware Deployment: A Trojan (Backdoor.PsEmpire) provided remote access, while JSCoinminer exploited system resources.
* Command & Control (C2): Attackers communicated externally using port 3333.
*Data Exfiltration: A BCC rule forwarded sensitive emails to an attacker-controlled address.
* Lateral Movement & Persistence: Unauthorized accounts (SVCVNC, Tomcat7) were created on the network.

Mapped to Cyber Kill Chain & MITRE ATT&CK:

* Cyber Kill Chain: From Reconnaissance (scanning AWS S3 buckets) to Actions on Objectives (data exfiltration).
* MITRE ATT&CK Techniques: Credential dumping, phishing, C2 communication, privilege escalation, and data exfiltration.

Tools Used:

* Splunk: Log analysis and attack timeline reconstruction.
* VirusTotal & MITRE ATT&CK: Malware classification and behavior analysis.
* System & Network Logs: Anomaly detection and correlation.

Key Takeaways:

* Enforce Multi-Factor Authentication (MFA) to prevent credential abuse.
* Restrict IAM privileges to minimize the attack surface.
* Monitor and block C2 traffic to disrupt external attacker communication.
* Deploy Endpoint Detection and Response (EDR) solutions to detect malware persistence.

This project enhanced my skills in threat hunting, security monitoring, and incident response. Feel free to connect if you’d like to discuss Blue Team strategies further.
