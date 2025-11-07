# 🛡️ Wazuh SIEM Setup & Configuration  
*A hands-on cybersecurity project demonstrating centralized log management, intrusion detection, and real-time alerting using Wazuh.*

---

## Project Overview
This project showcases the **deployment and configuration of the Wazuh SIEM platform**, designed to collect, analyze, and visualize security events from multiple systems.  

By setting up the **Wazuh Manager**, **Indexer**, **Dashboard**, and **Agents**, I created a small-scale **Security Operations Center (SOC)** environment capable of detecting, alerting, and analyzing endpoint activity in real time.

---

## Objectives
- Deploy a full **Wazuh 4.14 SIEM Stack** (Manager, Indexer, Dashboard)  
- Register **Linux (Kali)** and **Windows** agents for monitoring  
- Collect and analyze **system logs, authentication logs, and process data**  
- Visualize alerts through the **Wazuh Dashboard**  
- Demonstrate **SOC-level monitoring, threat detection, and investigation**

---

## Tools & Technologies

| Category | Tools / Components |
|-----------|--------------------|
| **SIEM Platform** | Wazuh 4.14 (Manager, Indexer, Dashboard) |
| **Virtualization** | VirtualBox |
| **Operating Systems** | Kali Linux, Windows 11 |
| **Log Sources** | Sysmon, Windows Event Logs, Auth.log |
| **Visualization** | Wazuh Dashboard |

---

## Skills Demonstrated

| Area | Skills Gained |
|------|----------------|
| **SIEM Management** | Installing and configuring Wazuh components |
| **Log Collection** | Ingesting Linux and Windows event logs |
| **Threat Detection** | Using built-in Wazuh rules and decoders to detect suspicious events from Windows and Linux systems |
| **SOC Practices** | Simulating real-world security monitoring workflows |
| **Linux Administration** | Managing services, networking, and permissions |

---

## Architecture Overview
        ┌──────────────────────────┐
        │      Endpoints / VMs     │
        │ ──────────────────────── │
        │  • Windows Agent         │
        │  • Linux Agent (Kali)    │
        │  • Suricata IDS Logs     │
        └────────────┬─────────────┘
                     │
                     ▼
        ┌────────────────────────────┐
        │     Wazuh Manager (OVA)    │
        │ ───────────────────────────│
        │ • Receives agent logs      │
        │ • Applies decoders/rules   │
        │ • Triggers alerts & events │
        └────────────┬───────────────┘
                     │
                     ▼
       ┌──────────────────────────────┐
       │       Wazuh Indexer          │
       │             │
       │ ─────────────────────────────│
       │ • Indexes security events    │
       │ • Supports queries & alerts  │
       └─────────── ┬────────────────┘
                    │
                    ▼
       ┌──────────────────────────────┐
       │        Wazuh Dashboard       │
       │             │
       │ ─────────────────────────────│
       │ • View alerts & dashboards   │
       │ • GeoIP & AbuseIPDB maps     │
       │ • Agent & rules management   │
       └──────────────────────────────┘


---

## Setup & Configuration Steps

### 1. Import the Wazuh OVA Appliance  
> ![Importing Wazuh OVA](https://github.com/OLADOTUN12/wazuh-siem-setup/blob/main/Wazuh-ova-imported.png?raw=true)

### 2. Install and Register Linux Agent (Kali)  
> ![Registering Kali Agent](https://github.com/OLADOTUN12/wazuh-siem-setup/blob/main/wazuh-agent%20-4.14.0-%20installation-%20kali%20linux.png?raw=true)![Registering Kali Agent](https://github.com/OLADOTUN12/wazuh-siem-setup/blob/main/wazuh-agent-%20running.png?raw=true)![Registering Kali Agent](https://github.com/OLADOTUN12/wazuh-siem-setup/blob/main/Configure-agent-%20connection-to-talk-manager.png?raw=true)![Registering Kali Agent](https://github.com/OLADOTUN12/wazuh-siem-setup/blob/main/Kali-linux-added-successfully-as-agent.png?raw=true)

### 3. Install and Register Windows Agent  
> ![Registering Windows Agent](https://github.com/OLADOTUN12/wazuh-siem-setup/blob/main/Window-wazuh-agent-registration.png?raw=true)

### 4. Access the Wazuh Dashboard  
> ![Wazuh Dashboard Login](https://github.com/OLADOTUN12/wazuh-siem-setup/blob/main/Screenshot%202025-11-06%20162818.png?raw=true)![Wazuh Dashboard Login](https://github.com/OLADOTUN12/wazuh-siem-setup/blob/main/Dashboard-view-showing-kali-and-window-agent-active.png?raw=true)

### 5. View Alerts and Security Events  
> ![Alerts View](https://github.com/OLADOTUN12/wazuh-siem-setup/blob/main/Alert-%20view.png?raw=true)

### 6. Vulnerability Detection Results  
> ![Vulnerability Detection](https://github.com/OLADOTUN12/wazuh-siem-setup/blob/main/Window-vulnerability.png?raw=true)

---

## Key Takeaways
- Gained hands-on experience in **SIEM deployment and management**  
- Learned how to **collect and correlate security logs** from multiple endpoints  
- Configured **real-time alerting and visualization** for system activity  
- Understood the **end-to-end SOC workflow** using open-source tools  

---

## Future Enhancements
- Integrate **Suricata IDS** for network threat detection  
- Add **GeoIP and AbuseIPDB enrichment** to dashboard alerts

