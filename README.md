# Omar | Cybersecurity

I’m a university student focused on blue-team work, detection engineering, and security automation. I use a Kali and Ubuntu lab to test attacks, inspect the logs they leave behind, and write detections I can explain.

This is where I keep the projects, queries, and notes from that work. Each writeup covers the setup, the detection logic, and the gaps I found along the way.

## Projects

- **[CI/CD Pipeline Security Auditor](https://github.com/notsobs/ci-cd-pipeline-security-auditor)** — Scans GitHub Actions for suspected secrets, mutable dependencies, injection patterns, and risky permissions. Includes vulnerable/corrected examples and automated tests.

- **[Custom SSH Intrusion Detection System](https://github.com/notsobs/Custom-IDS)** — A Python log analyzer for failed-login bursts and suspicious successful access. Includes a synthetic sample and the limits of IP-based correlation.

- **[SSH Brute-Force Detection](https://github.com/notsobs/SSH-bruteforce-detection)** — An isolated attack simulation with Splunk searches for failure bursts and suspicious authentication events.

- **[Port Scan Detection](https://github.com/notsobs/port-scan-detection)** — Nmap reconnaissance investigated through iptables logs, Filebeat, Elasticsearch, and Kibana.

- **[Web Attack Detection](https://github.com/notsobs/Web-Attacks-Detection)** — DVWA experiments and SPL queries for SQLi, XSS, and traversal, including the POST-body visibility gap.

## Tools used in these projects

- **Detection and investigation:** Splunk, SPL, Elasticsearch, Kibana, Filebeat.
- **Automation:** Python, regular expressions, YAML, Git, GitHub Actions.
- **Lab work:** Kali Linux, Ubuntu Server, VirtualBox, Nmap, Metasploit, DVWA, Apache, iptables.

## What I’m working on

Making detections more reliable: checking benign cases, documenting false positives, and being clear about what the available data cannot prove. I’m also extending that approach to CI/CD security and automated checks.

The lab writeups describe my recorded experiments. The auditor uses deliberately vulnerable test configurations; its sample credentials are fake.
