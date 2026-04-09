 Ransomware Incident Response Simulation (Wazuh SIEM)

Project Overview

This project demonstrates a full ransomware incident response simulation using Wazuh SIEM and a Windows 10 endpoint, mapped to the MITRE ATT&CK framework.

The objective is to showcase real-world SOC analyst and Blue Team skills, including detection, investigation, containment, eradication, recovery, and post-incident analysis.

This project is designed for entry to mid-level SOC / Blue Team roles

Objectives

Detect ransomware-related activity using Wazuh SIEM
 
 Analyze endpoint telemetry and security alerts
 
 Map attacker behavior to the MITRE ATT&CK framework
 
 Build a full ransomware kill chain timeline
 
 Perform structured Incident Response (IR)
 
 Produce professional SOC documentation


Lab Environment

Infrastructure

SIEM: Wazuh (All-in-One deployment)

SIEM OS: Ubuntu Server

Endpoint: Windows 10

Virtualization: VMware

System Resources

Ubuntu Server: 2GB RAM

Windows Endpoint: Wazuh Agent installed and active

Detection & Monitoring

Telemetry Sources

Windows Security Event Logs

PowerShell execution logs

File Integrity Monitoring (FIM)
 
 Agent status and heartbeat monitoring

Tools Used

Wazuh Dashboard

Wazuh Agent (Windows)

MITRE ATT&CK Framework


Ransomware Kill Chain (MITRE ATT&CK Mapping)

Phase | MITRE Tactic | Technique ID | Description 
 
 Initial Access | Initial Access | T1078 | Valid Accounts (Simulated) 
 
 Execution | Execution | T1059 | PowerShell Execution 
 
 Persistence | Persistence | T1547 | Autostart Execution (Monitored) 
 
 Privilege Escalation | Privilege Escalation | T1068 | Exploitation (Not Observed) 
 
 Defense Evasion | Defense Evasion | T1562 | Impair Defenses 
 
 Discovery | Discovery | T1083 | File & Directory Discovery 
 
 Impact | Impact | T1486 | Data Encrypted for Impact 
 
 Command & Control | Command and Control | T1071 | Application Layer Protocol (Monitored) 

Incident Response Workflow

Identification
 
 Suspicious PowerShell execution detected
 
 File Integrity Monitoring alerts indicated mass file modification
 
 Incident classified as Ransomware

Containment

 Infected endpoint isolated from the network (manual simulation)
 
 Log collection maintained for forensic evidence

 Eradication

 Malicious artifacts identified and removed (simulated)
 
 Compromised credentials reset

 Recovery
 
 Endpoint marked for reimaging
 
 System restoration from clean backup (simulated)

 Post-Incident Review
 
 Lessons learned documented
 
 Detection and monitoring improvements recommended

Incident Summary

Incident Type:Ransomware

Affected Host: Windows 10 Endpoint

Detection Tool: Wazuh SIEM

MITRE Impact Technique: T1486 – Data Encrypted for Impact

Status: Resolved


 Screenshots

( screenshots can be seen in docs/screenshots folder)

such as

![Wazuh Dashboard](docs/screenshots/dashboard.png)

![Active Agent](docs/screenshots/agent-active.png)

![Security Events](docs/screenshots/security-events.png)

![FIM Alerts](docs/screenshots/fim-alerts.png)


Key Takeaways

Demonstrates end-to-end SOC analyst workflow
Practical application of MITRE ATT&CK
Emphasizes documentation and response maturity

