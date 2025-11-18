# HF 2019 – Vulnerable Machine (Local VM)  
A Practical Pentesting Walkthrough & Analysis

This repository contains a clean and structured documentation of the **HF 2019 vulnerable machine**, which I deployed and tested locally inside my own virtual environment.  
The goal of this project is to demonstrate a full penetration-testing workflow using real attacker methodology, focusing on enumeration, exploitation, and credential compromise.

---

## 🔍 Machine Overview
HF 2019 is an intentionally vulnerable Linux-based machine that exposes weak authentication, outdated web components, and common misconfigurations.  
It is ideal for practicing:

- Network enumeration  
- Web vulnerability analysis  
- WordPress CMS assessment  
- Credential harvesting  
- Password cracking  
- SSH-based access escalation  

This machine was set up locally (not from HTB) and tested in a controlled lab environment.

---

## 🧭 Workflow Followed
The assessment was performed using a systematic attacker workflow:

1. **Identify the machine IP address**  
2. **Run a full Nmap port scan**  
3. **Run an aggressive scan for version details**  
4. **Analyze open ports & vulnerable services**  
5. **Check HTTP service and inspect the web page**  
6. **Identify CMS through page source**  
7. **Confirm WordPress using Wappalyzer**  
8. **Enumerate WordPress users using WPScan (API)**  
9. **Extract usernames & password hashes**  
10. **Crack hash using John the Ripper**  
11. **SSH into the machine with cracked credentials**  

This demonstrates a complete attack chain—from recon to foothold.

---

## 📌 Tools Used
- **Nmap** – Service & vulnerability enumeration  
- **Wappalyzer** – Web technology detection  
- **WPScan (API-based enumeration)** – WordPress assessment  
- **John the Ripper** – Password cracking  
- **SSH** – Final access  

---

## 🎯 Objective
The primary goal of this project is to show how a simple misconfigured environment can be exploited end-to-end:

**Find → Enumerate → Extract → Crack → Access**

The final result:  
✔️ **Successful SSH login using cracked credentials**

---

## ⚠️ Disclaimer
This machine is used solely for **ethical hacking practice**, **learning**, and **research** inside a safe and isolated virtual environment.  
Do not use these techniques outside authorized labs.

---
