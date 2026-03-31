<div align="center">

# 🐍 Python Automation & Scripting
### Weekly Mini-Projects — Mastering Python for Cybersecurity & SOC Automation

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Automation](https://img.shields.io/badge/Automation-22C55E?style=for-the-badge)](https://github.com/Aceknight4)
[![Cybersecurity](https://img.shields.io/badge/Cybersecurity-1B2A4A?style=for-the-badge)](https://github.com/Aceknight4)

> A structured series of Python mini-projects focused on building automation and scripting skills specifically for cybersecurity and SOC analyst roles.

</div>

---

## 🎯 Goal

Python is the #1 language for SOC automation, SIEM scripting, and security tooling. This repository documents my journey learning Python through hands-on cybersecurity-focused projects — each one building toward the skills used in [SentinelLite](https://github.com/Aceknight4/SentinelLite).

---

## 📚 Project Log

| Week | Project | Skills Practiced | Status |
|------|---------|-----------------|--------|
| 1 | Hello World & Variables | Basics, data types | ✅ Done |
| 2 | Profile Display | f-strings, lists, datetime | ✅ Done |
| 3 | File Handler | File I/O, read/write/append | ✅ Done |
| 4 | Log Generator | Functions, timestamps, loops | ✅ Done |
| 5 | Threat Detector | Regex, file parsing, dictionaries | ✅ Done |
| 6 | Port Scanner | Sockets, TCP, threading | ✅ Done |
| 7 | Password Checker | String analysis, policy logic | ✅ Done |
| 8 | Alerting Script | Email/Telegram notifications | 🔄 In Progress |
| 9 | Dashboard | Flask, HTML, data display | 🔄 In Progress |

---

## 💡 What I Learned Along the Way

**Week 1–2 (Foundations)**
- Variables, data types, f-strings, lists — the building blocks
- Why Python is the go-to language for security scripting

**Week 3–4 (File Operations)**
- How SIEM tools ingest and store log data
- Writing timestamped entries — the foundation of every log system

**Week 5 (Threat Detection Logic)**
- How Splunk and Wazuh detection rules actually work under the hood
- Regex patterns for extracting IPs, timestamps, and event types from logs
- Threshold-based alerting — the difference between noise and a real threat

**Week 6 (Networking in Python)**
- How TCP connections work at the socket level
- Building a port scanner from scratch — understanding what Nmap does internally

**Week 7 (Security Policy)**
- Password policy enforcement in code
- How PAM (Pluggable Authentication Modules) applies similar logic on Linux

---

## 🚀 How to Run

```bash
git clone https://github.com/Aceknight4/python-automation-and-scripting.git
cd python-automation-and-scripting

# Each week is in its own folder
cd week_05_threat_detector/
python3 threat_detector.py
```

No external dependencies for early weeks. Later weeks may require:
```bash
pip install requests flask
```

---

## 🔗 Where This Leads

These scripts directly evolved into:
- **[security-toolkit](https://github.com/Aceknight4/security-toolkit)** — Polished, structured versions of these scripts
- **[SentinelLite](https://github.com/Aceknight4/SentinelLite)** — Full SOC automation system using Suricata + ML + Flask

---

## 👤 Author

**Seppo Anel Graph Mbake**  
SOC Analyst | Blue Team Engineer | ISO 27001 Certified  
📧 [annelgraph46@gmail.com](mailto:annelgraph46@gmail.com)  
🔗 [LinkedIn](https://linkedin.com/in/seppo-anel-graph-mbake-03b736206)  
💻 [GitHub](https://github.com/Aceknight4)
