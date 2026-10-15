# Omar | Cybersecurity

I’m a university student focused on blue-team work, detection engineering, and security automation. I use a Kali and Ubuntu lab to test attacks, inspect the logs they leave behind, and write detections I can explain.

This is where I keep the projects, queries, and notes from that work. Each writeup covers the setup, the detection logic, and the gaps I found along the way.

## Projects

| Project | What I built | What I learned |
| --- | --- | --- |
| [CI/CD Pipeline Security Auditor](https://github.com/notsobs/ci-cd-pipeline-security-auditor) | Python auditor for GitHub Actions: suspected secrets, dependency pins, injection patterns, and risky permissions. Includes vulnerable/corrected examples and automated tests. | How to turn configuration risks into repeatable checks and useful findings. |
| [Custom SSH Intrusion Detection System](https://github.com/notsobs/Custom-IDS) | Python log analyzer that flags repeated SSH failures and later logins from a flagged source. | Sliding windows, log parsing, and the limits of IP-based correlation. |
| [SSH Brute-Force Detection](https://github.com/notsobs/SSH-bruteforce-detection) | An isolated SSH attack simulation with Splunk queries for failed logins and suspicious successful access. | Choosing thresholds and distinguishing an alert from evidence of compromise. |
| [Port Scan Detection](https://github.com/notsobs/port-scan-detection) | Nmap activity logged with iptables, shipped through Filebeat, and investigated in Elasticsearch and Kibana. | Detecting reconnaissance through distinct destination ports. |
| [Web Attack Detection](https://github.com/notsobs/Web-Attacks-Detection) | DVWA attack simulations and SPL queries for SQL injection, XSS, and path traversal. | URL decoding and the visibility lost when POST bodies are absent from access logs. |

## Tools used in these projects

- **Detection and investigation:** Splunk, SPL, Elasticsearch, Kibana, Filebeat.
- **Automation:** Python, regular expressions, YAML, Git, GitHub Actions.
- **Lab work:** Kali Linux, Ubuntu Server, VirtualBox, Nmap, Metasploit, DVWA, Apache, iptables.

## What I’m working on

Making detections more reliable: checking benign cases, documenting false positives, and being clear about what the available data cannot prove. I’m also extending that approach to CI/CD security and automated checks.

The lab writeups describe my recorded experiments. The auditor uses deliberately vulnerable test configurations; its sample credentials are fake.
