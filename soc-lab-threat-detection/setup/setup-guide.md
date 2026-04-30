# 🛠️ SOC Lab Setup Guide

## 📌 Objective
To build a controlled lab environment for simulating and detecting cyber attacks using a SIEM solution.

---

## 🖥️ Lab Architecture

- Attacker Machine: Kali Linux  
- Victim Machine: Windows 10  
- SIEM Server: Wazuh  

---

## ⚙️ Requirements

- VirtualBox  
- Minimum 8GB RAM (16GB recommended)  
- 50GB+ free storage  

---

## 🧱 Virtual Machine Setup

### 1. Kali Linux (Attacker)
- Installed Kali Linux on VirtualBox  
- Allocated 2GB RAM  
- Used for simulating attacks  

---

### 2. Windows 10 (Victim)
- Installed Windows 10 VM  
- Allocated 3 GB RAM  
- Enabled logging for security events  

---

### 3. Wazuh Server (SIEM)

Installed Wazuh using the official installation script:

``bash
curl -sO https://packages.wazuh.com/4.14/wazuh-install.sh
sudo bash wazuh-install.sh -a

---

-Accessed dashboard via browser
-Configured Wazuh agent on Windows machine
-🌐 Network Configuration
-All VMs connected to Internal Network
-Ensured communication between attacker, victim, and SIEM
-🔗 Agent Configuration
-Installed Wazuh agent on Windows
-Connected agent to Wazuh server
-Verified log forwarding

