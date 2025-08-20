# 🛡️ Wazuh SIEM – Analyzing an Infected Virtual Machine

This documentation outlines how to use **Wazuh**, a powerful open-source SIEM and security platform, to investigate and analyze a potentially **infected virtual machine (VM)**.  
It provides a workflow for detection, log collection, forensic analysis, and response.

---

## 📌 Overview

Wazuh provides:
- **Real-time log collection and correlation**
- **Intrusion detection (IDS)**
- **File integrity monitoring (FIM)**
- **Rootkit detection**
- **Incident response capabilities**

By deploying a Wazuh agent on a VM, you can gather forensic evidence and monitor malicious activity for deeper analysis.

---

## ⚙️ Setup

### 1. Deploy the Wazuh Agent on the VM
On the infected machine (Linux example):
```bash
curl -so wazuh-agent.sh https://packages.wazuh.com/4.x/wazuh-agent.sh
sudo bash wazuh-agent.sh --register-agent <WAZUH_MANAGER_IP>
sudo systemctl enable wazuh-agent
sudo systemctl start wazuh-agent
```


On Windows:

Download the Wazuh agent MSI
.

Register the agent to the Wazuh Manager.

Start the service via services.msc or PowerShell.

🔍 Analysis Workflow
1. Log Collection

System logs (auth, kernel, application events)

Security events (failed logins, privilege escalation)

Network activity (suspicious connections, ports in use)

File system changes (new/modified files)

2. Detection

Key Wazuh modules for VM investigation:

Syscheck (File Integrity Monitoring):
Detects new or altered files (e.g., malware dropped).

Rootcheck:
Scans for known rootkits, hidden processes, or kernel-level compromises.

OSSEC Rules:
Alerts on brute-force, malware behavior, persistence mechanisms, etc.

Vulnerability Detector:
Matches installed software with known CVEs.

3. Investigation

Use the Wazuh Dashboard (Kibana/Elastic) to:

Search alerts by timeframe:

agent.name: "infected-vm" AND rule.level >= 7


Inspect suspicious processes:

High CPU usage

Unusual parent-child process chains

Analyze network traffic:

Outbound connections to suspicious IPs

Unexpected open ports

Review privilege escalation attempts:

sudo misuse

Unauthorized user creation

4. Forensics & Threat Hunting

Correlate Wazuh alerts with external threat intel (VirusTotal, AbuseIPDB).

Identify persistence mechanisms:

Startup scripts

Registry run keys (Windows)

Cron jobs (Linux)

Export logs for deeper analysis:
```bash
/var/ossec/logs/alerts/alerts.json
```




