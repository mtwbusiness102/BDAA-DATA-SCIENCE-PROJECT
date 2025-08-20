# 🔐 SIEM Implementation with Wazuh

This project demonstrates the use of **Wazuh** as a Security Information and Event Management (SIEM) solution.  
It provides centralized **log collection, threat detection, compliance monitoring, and incident response**—making it a valuable tool for IT and cybersecurity projects.  

---

## 📌 Why Wazuh?
Wazuh is an open-source security platform that delivers:
- ✅ **Log Collection & Correlation** – Aggregates logs from servers, endpoints, and network devices  
- ✅ **Threat Detection** – Detects malware, brute-force attempts, anomalies, and suspicious activity  
- ✅ **Compliance Monitoring** – Helps meet standards like PCI DSS, HIPAA, GDPR, and ISO 27001  
- ✅ **Intrusion Detection (HIDS/NIDS)** – Monitors file integrity and network traffic  
- ✅ **Scalability** – Works for small IT environments and large enterprise infrastructures  

This makes Wazuh a **cost-effective SIEM** for IT teams to monitor and secure infrastructure.  

---

## 🏗️ Project Use Case
The goal of this project is to showcase how **Wazuh can be deployed in an IT environment** to improve security posture.  

**Use Case Example:**
- An IT organization wants centralized monitoring of:
  - Windows servers  
  - Linux endpoints  
  - Firewalls & network devices  
- Wazuh provides:
  - Unified log management  
  - Automated alerts for suspicious activity  
  - Dashboards for security visibility  
  - Compliance reporting  

---

## 📦 Installation & Setup



### 1. Install Wazuh Manager
```bash
curl -sO https://packages.wazuh.com/4.9/wazuh-install.sh
sudo bash wazuh-install.sh -a
```


### 2. Deploy Wazuh Agents
```bash
On endpoints (Linux, Windows, MacOS):

# Example: Linux agent installation
curl -sO https://packages.wazuh.com/4.9/wazuh-agent.sh
sudo bash wazuh-agent.sh
```
