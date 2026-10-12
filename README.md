# 🛡️ Cybersecurity & SOC Learning Journey

> Documenting my path from backend developer to SOC analyst: notes, labs, write-ups, and projects.

![Status](https://img.shields.io/badge/status-actively%20learning-brightgreen)
![Focus](https://img.shields.io/badge/focus-SOC%20%7C%20Blue%20Team-blue)
[![TryHackMe](https://img.shields.io/badge/TryHackMe-nohaabdulaziz373-red?logo=tryhackme&logoColor=white)](https://tryhackme.com/p/nohaabdulaziz373)
[![LetsDefend](https://img.shields.io/badge/LetsDefend-nohaa3mr-blue)](https://app.letsdefend.io/user/nohaa3mr)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-nohaamr710-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/nohaamr710)

## 👋 About This Repo

I'm a Computer Science student (graduating 2027) with a backend .NET background, now building skills in defensive security. This repo tracks what I learn, what I practice, and what I build, so everything here is backed by hands-on work, not just theory.

**Goal:** [e.g. Junior SOC Analyst / Security Engineer role by 2027]
**Currently learning:** LetsDefend SOC Analyst path (alert triage, log analysis, incident response)

---

## 🗺️ Roadmap

- [x] Cybersecurity fundamentals (LetsDefend: Cybersecurity for Students path)
- [x] Linux basics (TryHackMe: Linux Fundamentals Parts 1-3)
- [ ] Networking fundamentals
- [ ] LetsDefend SOC Analyst path 🔄 *(starting now)*
- [ ] Windows & Active Directory basics
- [ ] SIEM (Splunk / Wazuh / ELK)
- [ ] Incident response & threat hunting
- [ ] MITRE ATT&CK & Cyber Kill Chain
- [ ] Certification: [Security+ / CC / BTL1 / CySA+ — pick one]

---

## 📚 Notes

| # | Topic | Key takeaway |
|---|-------|--------------|
| 01 | [Networking fundamentals](./notes/01-networking.md) | OSI/TCP-IP, devices, NAT, VLAN, ARP; trace Source → Protocol → Destination |
| 02 | [Windows & Linux fundamentals](./notes/02-operating-systems.md) | Know normal paths, processes, services, persistence spots |
| 03 | [Network protocols](./notes/03-network-protocols.md) | TCP vs UDP, DNS, SSH, HTTP, DHCP and what abuse looks like |
| 04 | [Cryptography](./notes/04-cryptography.md) | Encryption vs hashing vs signatures solve different problems |
| 05 | [Malware analysis](./notes/05-malware-analysis.md) | Static vs dynamic analysis, safe triage in an isolated lab |
| 06 | [Malware traffic with Wireshark](./notes/06-malware-traffic-wireshark.md) | PCAP workflow: overview → pivot on host → patterns → correlate |
| 07 | [Investigating a SIEM alert](./notes/07-siem-alert-investigation.md) | An alert is a lead, not proof; validate, correlate, verdict |
| ⭐ | [Investigation chains cheat sheet](./cheatsheets/investigation-chains.md) | One-page Blue Team checklists |

-------|---------|------|
| CIA Triad & core concepts | One-line takeaway | [notes](./notes/fundamentals.md) |
| Networking (TCP/IP, DNS, HTTP) | One-line takeaway | [notes](./notes/networking.md) |
| Common attacks (phishing, SQLi, XSS…) | One-line takeaway | [notes](./notes/attacks.md) |
| *(add more)* | | |

---

## 🧪 Labs & Write-ups

| Date | Platform | Lab / Room | Skills Practiced | Write-up |
|------|----------|-----------|------------------|----------|
| 2026-10 | TryHackMe | Linux Fundamentals Part 1 | Shell navigation, files | [link](./labs/thm-linux-fundamentals-1.md) |
| 2026-10 | TryHackMe | Linux Fundamentals Part 2 | Permissions, processes | [link](./labs/thm-linux-fundamentals-2.md) |
| 2026-10 | TryHackMe | Linux Fundamentals Part 3 | Services, logs, automation | [link](./labs/thm-linux-fundamentals-3.md) |

**Each write-up should follow this structure:** Objective → Tools → Steps → Findings → What I learned.

---

## 🔧 Tools I've Used

| Category | Tools |
|----------|-------|
| Network analysis | Wireshark (PCAP analysis, LetsDefend course) |
| Operating systems | Linux CLI (TryHackMe), Windows CLI tools |
| SIEM / alerts | LetsDefend alert investigation (training) |
| *(add as you learn)* | Splunk, Wazuh, Sysmon, VirusTotal... |

----------|-------|
| SIEM | Splunk, Wazuh *(only list what you've actually used)* |
| Network | Wireshark, Nmap |
| Endpoint | Sysmon, Windows Event Viewer |
| Threat Intel | VirusTotal, AbuseIPDB, MITRE ATT&CK |
| Scripting | Python, PowerShell, Bash |

---

## 🧩 Projects

### [Project name, e.g. Home SOC Lab]
- **What:** One sentence.
- **Stack:** Wazuh + Sysmon + Windows VM
- **Result:** What it detected / what you learned.
- **Link:** [repo](#)

---

## 🏆 Certifications & Progress

- ✅ LetsDefend: Cybersecurity for Students (learning path), [add credential link]
- 🔄 LetsDefend: SOC Analyst path, in progress
- 🎯 [Target cert, e.g. Security+ / BTL1], target [month/year]

---

## 📂 Repo Structure

```
├── notes/        # 7 concept notes (networking → SIEM investigation)
├── labs/         # Lab and CTF write-ups (coming)
├── projects/     # Hands-on builds (home lab, detection rules, scripts)
├── cheatsheets/  # Quick references
└── README.md
```

---

## 📫 Connect

[LinkedIn](https://www.linkedin.com/in/nohaamr710) · [TryHackMe](https://tryhackme.com/p/nohaabdulaziz373) · [LetsDefend](https://app.letsdefend.io/user/nohaa3mr) · [Email](mailto:you@example.com)
