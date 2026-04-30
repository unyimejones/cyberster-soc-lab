# SOC Home Lab — Blue Team Internship
**Cyberster Blue Team Internship | Phase One**
---

## 📌 Overview
A fully documented Security Operations Centre (SOC) home lab 
built from scratch as part of the Cyberster Blue Team Internship 
(Phase One), focused on SOC Operations and SIEM Foundations.

The lab simulates a real enterprise SOC environment — covering 
threat detection, log management, intrusion detection, firewall 
configuration, and executive security reporting.
---

## 🖥️ Lab Architecture
| Component | Details |
|---|---|
| Hypervisor | VMware Workstation |
| Network | VMnet8 (NAT) + VMnet1 (Host-Only) |
| Wazuh Server | Ubuntu 24.04 LTS |
| Attacker Machine | Kali Linux |
| Windows Endpoint | Windows 10 |
| Linux Endpoint | Ubuntu 64-bit |
| Firewall/Gateway | pfSense CE 2.7.2 |
---

## 🛠️ Tools & Technologies
| Tool | Purpose |
|---|---|
| Wazuh SIEM | Log management, threat detection, dashboards |
| Suricata IDS | Network intrusion detection |
| pfSense CE | Firewall and gateway management |
| MITRE ATT&CK | Threat intelligence and rule mapping |
| VirusTotal API | File and hash reputation analysis |
| URLhaus | Threat feed integration |
| ipset / iptables | GeoIP-based traffic blocking |
| VMware Workstation | Lab virtualisation |
---

## 📅 Build Progress
### ✅ Week 1 — Lab Setup & SIEM Foundation
- Deployed VMware lab environment with 4 VMs
- Installed and configured Wazuh SIEM stack on Ubuntu 24.04
- Configured agent enrollment for Windows and Linux endpoints
- Verified log ingestion and dashboard functionality

### ✅ Week 2 — Detection Rules & File Integrity Monitoring
- Built 3 custom Wazuh detection rules mapped to MITRE ATT&CK:
  - T1136 — Create Account
  - T1110 — Brute Force
  - T1091 — Replication Through Removable Media
- Configured File Integrity Monitoring (FIM) on endpoints
- Tested rule triggers and verified alert generation

### ✅ Week 3 — Intrusion Detection & GeoIP Blocking
- Deployed Suricata IDS integrated with Wazuh via eve.json
- Wrote 3 custom Suricata detection rules
- Implemented GeoIP-based blocking using ipset and iptables
- Verified end-to-end alert flow from Suricata into Wazuh dashboard

### ✅ Week 4 — Advanced Integrations & Reporting
- Deployed pfSense CE 2.7.2 as VM gateway
- Integrated VirusTotal API (tested with EICAR standard test file)
- Configured MITRE ATT&CK module in Wazuh
- Added URLhaus threat feed integration
- Built custom SOC dashboard in Wazuh
- Produced executive-level security report with dark
  hacker-aesthetic format
---

## 🎯 MITRE ATT&CK Coverage
| Technique ID | Technique Name | Detection Method |
|---|---|---|
| T1136 | Create Account | Custom Wazuh rule |
| T1110 | Brute Force | Custom Wazuh rule |
| T1091 | Replication Through Removable Media | Custom Wazuh rule |
---

## 📄 Weekly Reports
| Week | Focus | Report |
|---|---|---|
| Week 1 | Lab Setup & SIEM Foundation | [View]Week1_Report_Cyberster_1.docx |
| Week 2 | Detection Rules & FIM | [View](./reports/week2-report.md) |
| Week 3 | IDS & GeoIP Blocking | [View](./reports/week3-report.md) |
| Week 4 | Advanced Integrations | [View](./reports/week4-report.md) |
---

## 🧠 Key Learnings
- How to architect and deploy a functional SOC environment
  from scratch on a personal machine
- Real-world SIEM configuration, tuning, and alert triage
- Writing and mapping custom detection rules to MITRE ATT&CK
- Network intrusion detection with Suricata
- Threat intelligence integration (VirusTotal, URLhaus)
- Executive security reporting for non-technical stakeholders
---

## 🔗 Related Projects
- [Network Vulnerability Assessment Lab](../alx-network-vuln-assessment)
- [Linux System Hardening Lab](../alx-linux-hardening)
---

*Cyberster Blue Team Internship — Phase One, 2026*  
*SOC Operations & SIEM Foundations*
