# 🚨 Incident Report – SSH Brute Force Attempt

## 📌 Incident Summary
A series of failed SSH login attempts were detected on the Wazuh server, indicating a potential brute-force attack.

---

## 🕒 Date & Time
Apr 29, 2026  

---

## 🖥️ Affected System
- Host: wazuh-server  
- Service: SSH (Port 22)  

---

## 🌐 Source Information
- Source IP: 192.168.29.67  
- Source Port: Multiple random ports  
- Target User: root  

---

## 🔍 Observations

- Multiple failed login attempts detected  
- High frequency of authentication failures  
- Same IP repeatedly targeting the root account  
- No successful login observed  

---

## 📊 Log Evidence

- Event: SSH authentication failure  
- Rule Level: 5 (Medium severity)  
- SIEM: Wazuh alerts triggered  

---

## 🧠 Analysis

The repeated login attempts from a single IP targeting the root account indicate a brute-force attack pattern.

The attack appears automated due to:
- High number of attempts  
- Consistent targeting behavior  

---

## ⚠️ Risk Assessment

- Risk Level: Medium  
- Potential Impact: Unauthorized access if credentials are compromised  

---

## 🛡️ Recommended Actions

- Disable root login over SSH  
- Implement account lockout policies  
- Use strong password policies  
- Enable multi-factor authentication (MFA)  
- Monitor repeated login attempts  

---

## ✅ Conclusion

The activity was identified as a simulated brute-force attack in a controlled lab environment. Detection and analysis were successfully performed using SIEM tools.

---

## 📸 Evidence

![Wazuh Logs](../screenshots/ssh-failed-log.png)
![Dashboard Alerts](../screenshots/wazuh-alert-dashboard.png)
