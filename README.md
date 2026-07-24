<div align="center">

# Omar — Cybersecurity - blue teaming

**Rebuilding hands-on cybersecurity skills from the ground up — every lab built, broken, debugged, and documented by me.**

![Focus](https://img.shields.io/badge/focus-blue%20team%20%2F%20detection-1f6feb?style=for-the-badge)
![Status](https://img.shields.io/badge/status-actively%20learning-brightgreen?style=for-the-badge)
![Based in](https://img.shields.io/badge/based%20in-Amman%2C%20Jordan-orange?style=for-the-badge)

</div>

---

## Quick Navigation

**[Projects](#projects)** — three end-to-end attack simulation + detection labs, full writeups included
**[Toolbox](#toolbox)** — what I actually use, not just what I've heard of
**[Background](#background)** — where I'm at and where I'm headed

---

## Projects

Each one follows the same shape: build a real attack chain, generate real log data, build real detection logic, document what broke and how it got fixed. No canned datasets — every log line in every project came from an attack I actually ran myself.

| Project | Info | What it demonstrates |
|---|---|---|
| **[🔐 SSH Brute-Force Detection](https://github.com/notsobs/SSH-bruteforce-detection)** — SSH brute force, caught in Splunk | ![Splunk](https://img.shields.io/badge/Splunk-000000?style=flat-square&logo=splunk&logoColor=white) ![Difficulty](https://img.shields.io/badge/difficulty-beginner-brightgreen?style=flat-square) | Threshold-based SPL alerting, failed→success correlation, and hands-on debugging of OpenSSH's `PerSourcePenalties`/`MaxAuthTries` defenses |
| **[🛡️ Port Scan Detection](https://github.com/notsobs/port-scan-detection)** — Nmap scans caught via the ELK stack | ![Elastic](https://img.shields.io/badge/Elastic-005571?style=flat-square&logo=elasticsearch&logoColor=white) ![Difficulty](https://img.shields.io/badge/difficulty-beginner-brightgreen?style=flat-square) | Custom GROK ingest pipeline, iptables logging, Kibana threshold alerting on distinct ports touched per source IP |
| **[🎯 Web Attack Detection](https://github.com/notsobs/web-attack-detection)** — Web Attacks detected via splunk| ![Splunk](https://img.shields.io/badge/Splunk-000000?style=flat-square&logo=splunk&logoColor=white) ![Difficulty](https://img.shields.io/badge/difficulty-beginner--intermediate-yellow?style=flat-square) | Multi-vector web attack classification in SPL, plus a documented real limitation (POST-body blind spot in standard access logs) |

*More going up as I finish them.*

---

## Toolbox - more are added when documented

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

![Nmap](https://img.shields.io/badge/Nmap-000000?style=flat-square)
![Metasploit](https://img.shields.io/badge/Metasploit-2596CD?style=flat-square)
![Burp Suite](https://img.shields.io/badge/Burp%20Suite-FF6633?style=flat-square)
![Hydra](https://img.shields.io/badge/Hydra-red?style=flat-square)
![Hashcat](https://img.shields.io/badge/Hashcat-000000?style=flat-square)
![Gobuster/ffuf](https://img.shields.io/badge/Gobuster%20%2F%20ffuf-333333?style=flat-square)
![John the Ripper](https://img.shields.io/badge/John%20the%20Ripper-black?style=flat-square)
![sqlmap](https://img.shields.io/badge/sqlmap-orange?style=flat-square)

![Splunk](https://img.shields.io/badge/Splunk-000000?style=flat-square&logo=splunk&logoColor=white)
![Elasticsearch](https://img.shields.io/badge/Elasticsearch-005571?style=flat-square&logo=elasticsearch&logoColor=white)
![Kibana](https://img.shields.io/badge/Kibana-005571?style=flat-square&logo=kibana&logoColor=white)
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=flat-square&logo=wireshark&logoColor=white)
![Autopsy](https://img.shields.io/badge/Autopsy-2E3440?style=flat-square)
![Volatility](https://img.shields.io/badge/Volatility-6E4C13?style=flat-square)

![iptables](https://img.shields.io/badge/iptables-EE0000?style=flat-square)
![Fail2ban](https://img.shields.io/badge/Fail2ban-282828?style=flat-square)
![Apache](https://img.shields.io/badge/Apache-D22128?style=flat-square&logo=apache&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![MariaDB](https://img.shields.io/badge/MariaDB-003545?style=flat-square&logo=mariadb&logoColor=white)

![Kali](https://img.shields.io/badge/Kali%20Linux-557C94?style=flat-square&logo=kalilinux&logoColor=white)
![Ubuntu](https://img.shields.io/badge/Ubuntu-E95420?style=flat-square&logo=ubuntu&logoColor=white)


---

## Background

University student, Cyber security track. Currently deciding on a final project — Any help/recommondations would be appreciated.
---

<div align="center">
<i>Winning only.</i>
</div>
