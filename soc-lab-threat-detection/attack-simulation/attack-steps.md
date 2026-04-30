# Attack Simulation – SSH Brute Force Attempt

## 🎯 Objective
To simulate unauthorized login attempts on a target system and generate security logs for detection and analysis.

---

## 🖥️ Environment Setup

- Attacker Machine: Kali Linux  
- Target Machine: Wazuh Server  
- Target IP: 192.168.29.139  
- Protocol: SSH (Port 22)  

---

## ⚙️ Tools Used

- Hydra (for login attempts)  
- Wordlist: rockyou.txt  

---

## 🚀 Attack Execution

1. Navigated to wordlist directory:
   cd /usr/share/wordlists/

2. Extracted wordlist:
   gunzip rockyou.txt.gz

3. Initiated login attempts:
   hydra -l root -P /usr/share/wordlists/rockyou.txt ssh://192.168.29.139

---

## 🔍 Observations

- Multiple login attempts were made against the target system  
- Targeted username: root  
- High number of attempts within short time  
- Authentication attempts failed  

---

## ⚠️ Impact

- Generated repeated failed login logs  
- Triggered alerts in SIEM (Wazuh)  
- Simulated brute-force attack behavior  

---

## 🧠 Key Learning

- Brute-force attacks involve repeated login attempts  
- SIEM tools can detect abnormal login patterns  
- Monitoring failed authentication is critical for security  

---

## 📌 Note

This simulation was performed in a controlled lab environment for educational purposes only.
