# SIEM Homelab Project

## Table of Contents
1. [Objective](#objective)
2. [Key Skills](#key-skills)
3. [Tools](#tools)
4. [Project Highlights](#project-highlights)
   - [Nmap Scan Detection Alert Rule](#1-nmap-scan-detection-alert-rule)
   - [Event Monitoring During Penetration Testing](#2-event-monitoring-during-penetration-testing)
   - [Attack Simulation Using Hydra for SSH Brute-Force Detection](#3-attack-simulation-using-hydra-for-ssh-brute-force-detection)
   - [Email Alert Notification for SSH Brute-Force Attack](#4-email-alert-notification-for-ssh-brute-force-attack)
5. [Challenges and Solutions](#challenges-and-solutions)
6. [Key Takeaways](#key-takeaways)

---

## Objective
This project involves building a Security Information and Event Management (SIEM) system to detect and respond to cyber threats. Through analyzing network logs and simulating attacks, I gained hands-on experience with security monitoring, alert configuration, and incident response.

## Key Skills
- 🛠️ **SIEM Setup and Configuration**: Configured Elastic SIEM for centralized log management and monitoring.
- 🔍 **Log Analysis**: Detecting threats through multi-source log review.
- 🧩 **Data Normalization**: Consistent log parsing for reliable analysis.
- ⚠️ **Custom Alerts**: Rules to detect high-risk actions like brute-force and scans.
- 🚨 **Incident Response**: Real-time alerts and notifications for rapid response.
- 📊 **Data Visualization**: Dashboards to highlight trends and anomalies.
- 🌐 **Network Protocols**: Recognizing patterns in network behavior.
- 📬 **Automated Notifications**: Real-time alerts to security personnel.

## Tools
- **Elastic SIEM**: Used Elastic Stack to set up a SIEM server for log collection, alerting, and monitoring, providing a centralized platform for detecting and responding to threats.
- **Kali Linux VM**: Platform for performing penetration testing.
- **Hydra**: Used for simulating SSH brute-force attacks.
- **Nmap**: Utilized for network scanning and reconnaissance to simulate potential attack vectors.

## Project Highlights

---

### 1. Nmap Scan Detection Alert Rule
<div align="center">
  <img src="https://github.com/user-attachments/assets/b7fd5bcd-9474-4b3c-a05c-3694381a462e" alt="Nmap Scan Detection">
</div>

*Custom alert rule set up to detect and log Nmap scanning activity, helping track reconnaissance actions in the network.*

**Description**: I configured a custom alert rule to detect Nmap activity. This rule flagged any Nmap usage as potential reconnaissance, which is commonly associated with network probing by attackers. The SIEM displayed these alerts prominently, showcasing how specific rules can enhance threat detection for high-risk activities.

---

### 2. Event Monitoring During Penetration Testing
<div align="center">
  <img src="https://github.com/user-attachments/assets/d64e5bdf-a090-4900-b308-378a441af683" alt="Event Monitoring">
</div>

*Real-time event graph showing spikes in network activity during Nmap scans on the Kali VM.*

**Description**: I used Nmap on a Kali VM to simulate network scanning, which generated noticeable spikes in network traffic. The SIEM system captured and visualized this activity in real time, highlighting abnormal traffic patterns. This test demonstrated the SIEM’s ability to monitor network reconnaissance, providing early insights into potential threats.

---

### 3. Attack Simulation Using Hydra for SSH Brute-Force Detection
<div align="center">
  <img src="https://github.com/user-attachments/assets/319ac522-55fa-41b3-bfbe-7577220ab22f" alt="Hydra SSH Attack">
</div>

*SSH brute-force attack simulation using Hydra, detected and logged by the SIEM system.*

**Description**: Using Hydra, I simulated a brute-force attack on SSH to test the SIEM’s detection capabilities. The SIEM accurately logged each login attempt, creating a clear audit trail of the attack. This confirmed that the system could identify and record unauthorized access attempts effectively, a crucial feature for forensic analysis.

---

### 4. Email Alert Notification for SSH Brute-Force Attack
<div align="center">
  <img src="https://github.com/user-attachments/assets/a7e3b0f4-a2e9-4e4c-94d2-8c737fcebdd1" alt="Email Alert Notification">
</div>

*Automated email notification received upon detecting an SSH brute-force attack, alerting security personnel in real time.*

**Description**: I simulated an SSH brute-force attack using Hydra, and the SIEM was configured to send an immediate email alert upon detection. This real-time notification provided essential information about the attack, enabling prompt response. Receiving an email directly from the SIEM demonstrated the system’s ability to escalate alerts to designated personnel quickly, a critical feature in active security monitoring.

---

## Challenges and Solutions
- **Balancing Alert Sensitivity**: Finding the right sensitivity for alerts was challenging, as too many false positives could overwhelm the system. I tested and adjusted alert settings to reduce noise while ensuring significant threats were detected accurately, improving the SIEM's overall effectiveness.
  
---

## Key Takeaways
This project reinforced the importance of:
- **SIEM configuration** for comprehensive security monitoring.
- **Custom alert rules** for enhanced threat detection.
- **Real-time alerting** to enable fast responses during potential security incidents.
