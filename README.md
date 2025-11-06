# 🛡️ Wazuh SIEM Setup & Configuration  
*A hands-on cybersecurity project demonstrating centralized log management, intrusion detection, and real-time alerting using Wazuh.*

---

## 📘 Project Overview
This project showcases the **deployment and configuration of the Wazuh SIEM platform**, designed to collect, analyze, and visualize security events from multiple systems.  

By setting up the **Wazuh Manager**, **Indexer**, **Dashboard**, and **Agents**, I created a small-scale **Security Operations Center (SOC)** environment capable of detecting, alerting, and analyzing endpoint activity in real time.

---

## 🎯 Objectives
- Deploy a full **Wazuh 4.14 SIEM Stack** (Manager, Indexer, Dashboard)  
- Register **Linux (Kali)** and **Windows** agents for monitoring  
- Collect and analyze **system logs, authentication logs, and process data**  
- Visualize alerts through the **Wazuh Dashboard**  
- Demonstrate **SOC-level monitoring, threat detection, and investigation**

---

## 🧰 Tools & Technologies

| Category | Tools / Components |
|-----------|--------------------|
| **SIEM Platform** | Wazuh 4.14 (Manager, Indexer, Dashboard) |
| **Virtualization** | VirtualBox |
| **Operating Systems** | Kali Linux, Windows 11 |
| **Log Sources** | Sysmon, Windows Event Logs, Auth.log |
| **Visualization** | Wazuh Dashboard |

---

## 🧠 Skills Demonstrated

| Area | Skills Gained |
|------|----------------|
| **SIEM Management** | Installing and configuring Wazuh components |
| **Log Collection** | Ingesting Linux and Windows event logs |
| **Threat Detection** | Using built-in Wazuh rules and decoders to detect suspicious events from Windows and Linux systems |
| **SOC Practices** | Simulating real-world security monitoring workflows |
| **Linux Administration** | Managing services, networking, and permissions |

---

## 🧩 Architecture Overview
*(You can add a simple diagram here — optional but impactful)*  
Example:  
> ![Wazuh Architecture Diagram](images/wazuh-architecture.png)

---

## 🖥️ Setup & Configuration Steps


### 1. Import the Wazuh OVA Appliance  
> ![Importing Wazuh OVA](https://github.com/OLADOTUN12/wazuh-siem-setup/blob/main/Wazuh-ova-imported.png?raw=true)

### 2. Install and Register Linux Agent (Kali)  
> ![Registering Kali Agent](images/wazuh-agent-kali.png)

### 3. Access the Wazuh Dashboard  
> ![Wazuh Dashboard Login](images/wazuh-dashboard-login.png)

### 4. Install and Register Windows Agent  
> ![Registering Windows Agent](images/wazuh-agent-windows.png)

### 5. View Alerts and Security Events  
> ![Alerts View](images/wazuh-alerts-view.png)

### 6. Vulnerability Detection Results  
> ![Vulnerability Detection](images/wazuh-vuln-detection.png)

---

## 📊 Sample Dashboard Views

| View | Description |
|------|--------------|
| ![Agent Summary](images/agent-summary.png) | Shows connected agents and their status |
| ![Threat Detection](images/threat-detection.png) | Displays detected threats categorized by severity |
| ![Vulnerability Results](images/vuln-results.png) | Lists CVEs detected on endpoints with severity ratings |

---

## 🔍 Key Takeaways
- Gained hands-on experience in **SIEM deployment and management**  
- Learned how to **collect and correlate security logs** from multiple endpoints  
- Configured **real-time alerting and visualization** for system activity  
- Understood the **end-to-end SOC workflow** using open-source tools  

---

## 🧾 Future Enhancements
- Integrate **Suricata IDS** for network threat detection  
- Add **GeoIP and AbuseIPDB enrichment** to dashboard alerts  
- Automate agent deployment with **Ansible or Bash scripts**

---

## 📸 Folder Structure

