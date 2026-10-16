# Hey, I'm Omar 👋

I'm a university student learning cybersecurity by building things and seeing what shows up in the logs. Most of that happens in my home lab: Kali on one side, an Ubuntu server on the other, and a lot of figuring out why something didn't work.

I'm especially interested in the defensive side. Running an attack is one part; understanding what it leaves behind and writing a useful detection is the part I want to get better at.

## What I've been building

- **[CI/CD Pipeline Security Auditor](https://github.com/notsobs/ci-cd-pipeline-security-auditor)** — A Python tool for spotting risky GitHub Actions configurations: hardcoded secrets, unpinned actions, unsafe shell inputs, and overly broad permissions. Includes insecure examples and their fixes.

- **[Custom SSH Intrusion Detection System](https://github.com/notsobs/Custom-IDS)** — My own Python SSH log analyzer. It looks for repeated login failures and flags successful access from suspicious IPs.

- **[SSH Brute-Force Detection](https://github.com/notsobs/SSH-bruteforce-detection)** — Simulating SSH attacks in the lab, then using Splunk to find the failed logins and suspicious activity.

- **[Port Scan Detection](https://github.com/notsobs/port-scan-detection)** — Following an Nmap scan through firewall logs into Elasticsearch and Kibana.

- **[Web Attack Detection](https://github.com/notsobs/Web-Attacks-Detection)** — Trying SQL injection, XSS, and directory traversal against DVWA, then checking what the logs actually let me detect.

## Things I use

Python · Linux · Splunk / SPL · Elasticsearch · Kibana · Filebeat · GitHub Actions · Nmap · VirtualBox

## Still figuring out

How to make detections useful without flagging everything. I'm working on testing normal activity alongside attacks, understanding false positives, and being clearer about what a log can and can't tell me.

These repos are my working notes as much as they're a portfolio. Each one has the setup, what I tried, and the limitations I found. There's more to learn, and I'll keep adding to them as I go.
