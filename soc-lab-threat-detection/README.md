# SOC Lab – Threat Detection & Analysis

## 📌 Overview
This project demonstrates a hands-on Security Operations Center (SOC) lab built using Wazuh, Kali Linux, and Windows.

The lab simulates real-world cyber attacks and focuses on detecting and analyzing them using SIEM.

---

## 🧠 Architecture

Attacker → Kali Linux  
Victim → Windows Machine  
SIEM → Wazuh Server  

---

## ⚔️ Attacks Simulated

- SSH brute-force attack  
- Failed login attempts  
- Authentication failures  

---

## 🔍 Detection & Analysis

- Monitored logs using Wazuh dashboard  
- Identified repeated failed login attempts  
- Analyzed SSH authentication failure logs  
- Correlated attack patterns using SIEM  

---

## 📸 Screenshots

### 🔹 Attack from Kali Linux
![Kali Attack](screenshots/kali-bruteforce-attack.png)

### 🔹 Wazuh Dashboard Alerts
![Wazuh Dashboard](screenshots/wazuh-alert-dashboard.png)

### 🔹 SSH Failed Login Logs
![Logs](screenshots/ssh-failed-log.png)

### 🔹 Wazuh Server Status
![Wazuh VM](screenshots/wazuh-server-status.png)

---

## 📄 Incident Report (Summary)

- Source IP: Internal attacker machine  
- Target: Wazuh Server  
- Attack Type: SSH brute-force attempt  
- Observation: Multiple failed login attempts detected  
- Conclusion: Suspicious activity identified and analyzed  

---

## 🛠️ Tools Used

- Wazuh (SIEM)  
- Kali Linux  
- VirtualBox  
- Windows VM  

---

## 🚀 Key Skills Demonstrated

- Log analysis  
- Threat detection  
- SIEM monitoring  
- Incident investigation  

---

## 📌 Conclusion

This project demonstrates practical SOC analyst skills by simulating attacks, detecting threats, and analyzing logs in a controlled lab environment.
