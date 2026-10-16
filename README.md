# Hey, I'm Omar 👋

I'm a university student learning cybersecurity by building things and seeing what shows up in the logs. Most of that happens in my home lab: Kali on one side, an Ubuntu server on the other, and a lot of figuring out why something didn't work.

I'm especially interested in the defensive side. Running an attack is one part; understanding what it leaves behind and writing a useful detection is the part I want to get better at.

## What I've been building

[Security tools](#security-tools) · [Detection labs](#detection-labs) · [Things I use](#things-i-use)

The levels are my rough guide to project complexity: **Beginner** covers a focused workflow, **Beginner–Intermediate** combines several steps or concepts, and **Intermediate** adds more integration and testing.

### Security tools

#### [CI/CD Pipeline Security Auditor](https://github.com/notsobs/ci-cd-pipeline-security-auditor)

![Level: Intermediate](https://img.shields.io/badge/level-intermediate-F59E0B?style=flat-square) ![Type: Python tool](https://img.shields.io/badge/type-Python%20tool-3776AB?style=flat-square)

A Python tool that checks GitHub Actions for suspected secrets, unpinned actions, unsafe shell inputs, and risky permissions. It runs in CI too, so the workflow gets checked whenever I push.

**Skills:** YAML parsing, security rules, automated tests, GitHub Actions.

[Try the examples](https://github.com/notsobs/ci-cd-pipeline-security-auditor#run-the-lab) · [Read the report](https://github.com/notsobs/ci-cd-pipeline-security-auditor/blob/main/REPORT.md)

#### [Custom SSH Intrusion Detection System](https://github.com/notsobs/Custom-IDS)

![Level: Beginner–Intermediate](https://img.shields.io/badge/level-beginner--intermediate-0D9488?style=flat-square) ![Type: Python tool](https://img.shields.io/badge/type-Python%20tool-3776AB?style=flat-square)

My own SSH log analyzer, taking an idea from the Splunk lab and building it in Python. It counts failures in a sliding window and flags later successful logins from an alerted IP for review.

**Skills:** regex, log parsing, time windows, event correlation.

[Try the sample log](https://github.com/notsobs/Custom-IDS#run-it)

### Detection labs

#### [SSH Brute-Force Detection](https://github.com/notsobs/SSH-bruteforce-detection)

![Level: Beginner](https://img.shields.io/badge/level-beginner-22C55E?style=flat-square) ![Type: Splunk lab](https://img.shields.io/badge/type-Splunk%20lab-000000?style=flat-square)

A starting point for following an attack into the logs: generate SSH login attempts in an isolated lab, then investigate failures and successful access with Splunk.

**Skills:** Linux authentication logs, SPL, threshold searches.

[Read the lab](https://github.com/notsobs/SSH-bruteforce-detection#workflow) · [Browse the queries](https://github.com/notsobs/SSH-bruteforce-detection/tree/main/spl-queries)

#### [Port Scan Detection](https://github.com/notsobs/port-scan-detection)

![Level: Beginner–Intermediate](https://img.shields.io/badge/level-beginner--intermediate-0D9488?style=flat-square) ![Type: Elastic lab](https://img.shields.io/badge/type-Elastic%20lab-005571?style=flat-square)

Following an Nmap scan through iptables logs, Filebeat, Elasticsearch, and Kibana. The detection looks for a source reaching many different destination ports.

**Skills:** firewall logging, log ingestion, Grok parsing, cardinality alerts.

[Read the lab](https://github.com/notsobs/port-scan-detection#lab-setup)

#### [Web Attack Detection](https://github.com/notsobs/Web-Attacks-Detection)

![Level: Beginner–Intermediate](https://img.shields.io/badge/level-beginner--intermediate-0D9488?style=flat-square) ![Type: Splunk lab](https://img.shields.io/badge/type-Splunk%20lab-000000?style=flat-square)

Testing SQL injection, XSS, and file inclusion against DVWA, then writing searches around the Apache logs. The biggest lesson: a missing POST body means a missing piece of the investigation.

**Skills:** HTTP logs, URL decoding, SPL patterns, visibility gaps.

[Read the lab](https://github.com/notsobs/Web-Attacks-Detection#inputs-tested) · [Browse the queries](https://github.com/notsobs/Web-Attacks-Detection/tree/main/spl-queries)

## Things I use

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Kali Linux](https://img.shields.io/badge/Kali%20Linux-557C94?style=flat-square&logo=kalilinux&logoColor=white)
![Ubuntu](https://img.shields.io/badge/Ubuntu-E95420?style=flat-square&logo=ubuntu&logoColor=white)
![Splunk / SPL](https://img.shields.io/badge/Splunk%20%2F%20SPL-000000?style=flat-square&logo=splunk&logoColor=white)
![Elasticsearch](https://img.shields.io/badge/Elasticsearch-005571?style=flat-square&logo=elasticsearch&logoColor=white)
![Kibana](https://img.shields.io/badge/Kibana-005571?style=flat-square&logo=kibana&logoColor=white)
![Filebeat](https://img.shields.io/badge/Filebeat-005571?style=flat-square&logo=beats&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Nmap](https://img.shields.io/badge/Nmap-000000?style=flat-square)
![VirtualBox](https://img.shields.io/badge/VirtualBox-2F61B4?style=flat-square&logo=virtualbox&logoColor=white)

## Still figuring out

How to make detections useful without flagging everything. I'm working on testing normal activity alongside attacks, understanding false positives, and being clearer about what a log can and can't tell me.

These repos are my working notes as much as they're a portfolio. Each one has the setup, what I tried, and the limitations I found. There's more to learn, and I'll keep adding to them as I go.
