# 🔐 Wazuh SIEM SOC Home Lab

## 📌 Overview
This project demonstrates a hands-on Security Operations Center (SOC) home lab built using Wazuh SIEM. A Windows endpoint was integrated with a Wazuh server to monitor system activity, detect threats, and analyze security events.

The lab simulates real-world SOC workflows including log ingestion, threat detection, and event investigation.

---

## 🛠️ Technologies Used
- Wazuh SIEM
- Ubuntu (Wazuh Server)
- Windows 11 (Endpoint)
- VirtualBox
- PowerShell

---

## 🧱 Lab Architecture
- **Wazuh Server (Ubuntu VM)** – Central log collection and analysis
- **Windows Endpoint (VM)** – Generates security events
- **Wazuh Agent** – Sends logs from endpoint to server

---

## 🔍 Key Features

### ✅ Endpoint Monitoring
- Connected Windows agent to Wazuh server
- Verified active agent communication and log ingestion

---

### 🚨 Brute Force Detection
- Simulated failed login attempts on Windows
- Detected authentication failures in Wazuh

### 📂 File Integrity Monitoring (FIM)
- Configured syscheck to monitor file changes
- Triggered alerts by creating/modifying files

**Detected Events:**
- File added
- File modified
- Integrity checksum changes

---

### 🧠 Threat Hunting & Log Analysis
- Used Wazuh Threat Hunting dashboard to analyze events
- Investigated logs using detailed JSON view

**Example Insight:**
- File: `C:\Users\Public\test.txt`
- Change detected: size and hash modified
- Event type: integrity change

---

### 🧬 MITRE ATT&CK Mapping
- Observed alerts mapped to MITRE ATT&CK tactics
- Example categories: Defense Evasion, Impact

---

## 🎯 Skills Demonstrated
- SIEM deployment and configuration
- Endpoint monitoring and log analysis
- Threat detection (brute-force attacks)
- File integrity monitoring (FIM)
- Security event investigation (JSON logs)
- MITRE ATT&CK awareness

---

## 🚀 How to Reproduce (High-Level)
1. Set up Ubuntu VM and install Wazuh server
2. Set up Windows VM and install Wazuh agent
3. Connect agent to Wazuh manager
4. Generate events:
   - Failed login attempts
   - File creation/modification
5. Analyze logs in Wazuh dashboard

---

## 📸 Screenshots
- Agent active status
- Failed login events
- File integrity monitoring alerts
- Event detail (JSON view)

---

## 📈 Future Improvements
- Add multiple endpoints (Linux + Windows)
- Simulate malware detection (EICAR file)
- Implement alert notifications
- Automate incident response

---

## 💼 Resume Bullet
- Built a SOC home lab using Wazuh SIEM to monitor a Windows endpoint, detect brute-force login attempts, and implement file integrity monitoring for real-time threat detection and analysis.

---

## 🎤 Key Takeaway
This project demonstrates practical experience with SIEM tools, including detecting, analyzing, and investigating security events in a simulated SOC environment.
