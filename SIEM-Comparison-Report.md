<div align="center">

# 📊 Comparative Analysis of SIEM Solutions

## Splunk Enterprise · ELK Stack · Graylog

![Project Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)
![SIEM](https://img.shields.io/badge/SIEM-Comparative%20Analysis-blue?style=for-the-badge&logo=elasticsearch)
![Splunk](https://img.shields.io/badge/Splunk-Enterprise-00ADD8?style=for-the-badge&logo=splunk)
![ELK](https://img.shields.io/badge/ELK-Stack-005571?style=for-the-badge&logo=elastic)
![Graylog](https://img.shields.io/badge/Graylog-Open%20Source-FF3633?style=for-the-badge&logo=graylog)

![Security](https://img.shields.io/badge/Security-SOC%20Operations-purple?style=flat-square&logo=security)
![Incident Response](https://img.shields.io/badge/Incident%20Response-Case%20%23147-orange?style=flat-square)
![Cyber Kill Chain](https://img.shields.io/badge/Cyber%20Kill%20Chain-Mapped-red?style=flat-square)
![TheHive](https://img.shields.io/badge/TheHive-Ticketing%20Integrated-yellow?style=flat-square)

**Prepared by:** Yuri Montano  
**Date:** March 2026

</div>


## Table of Contents

1. Introduction  
2. Objective  
3. Splunk Overview  
4. ELK Stack Overview  
5. Graylog Overview  
6. Hands-On Implementation  
7. Comparison of SIEM Solutions 
8. Real-World Case Study: Incident #147 
9. Use Cases 
10. Security Considerations 
11. Conclusion 
12. Project Summary for CV / Portfolio 
---

## 1. Introduction

In modern enterprise environments, the increasing complexity of IT infrastructures and the growing number of cyber threats make security monitoring a critical component of any organization. Security Information and Event Management (SIEM) solutions play a key role by collecting, analyzing, and correlating log data from multiple sources in order to detect suspicious activities and respond to security incidents in real time.

SIEM platforms provide organizations with enhanced visibility over their systems, enabling security teams to identify potential threats, investigate incidents, and ensure compliance with security policies and regulations. As cyberattacks become more sophisticated, the adoption of efficient and scalable SIEM solutions is essential for maintaining a strong security posture.

This project focuses on the comparative analysis of three widely used SIEM solutions: Splunk, the ELK Stack (Elasticsearch, Logstash, and Kibana), and Graylog. These tools differ in terms of architecture, cost, complexity, and use cases, making them suitable for different types of environments. The objective of this study is to evaluate these solutions based on their features, usability, performance, and security capabilities, in order to identify their strengths, limitations, and most appropriate use cases.

---

## 2. Objective

The primary objective of this project is to conduct a comprehensive comparative analysis and practical evaluation of three leading Security Information and Event Management (SIEM) solutions: Splunk, ELK Stack (Elasticsearch, Logstash, Kibana), and Graylog.

This study focuses on several critical dimensions that define the effectiveness of a SIEM platform, including:

- **Architecture:** Understanding the underlying design, components, and deployment models of each solution.
- **Key Features:** Examining the core functionalities such as search capabilities, alerting mechanisms, visualization tools, and integration options.
- **Ease of Use:** Assessing the learning curve, interface intuitiveness, and operational complexity for security teams.
- **Scalability:** Evaluating how each platform performs as data volume and organizational size grow.
- **Security Capabilities:** Analyzing detection accuracy, correlation rules, threat intelligence integration, and incident response support.

Beyond the technical evaluation, this project aims to identify the specific strengths and limitations of each solution when deployed in different operational contexts ranging from small businesses with limited resources to large enterprises operating dedicated Security Operations Centers (SOCs).

Through hands-on implementation, real-world incident investigation, and research-based analysis, this study provides actionable insights to help organizations select the SIEM solution that best aligns with their technical requirements, team expertise, and budget constraints.

Ultimately, this project serves as both a technical reference for SIEM selection and a demonstration of practical cybersecurity skills applicable to real-world security operations.

---


## 3. Splunk Overview

<img width="638" height="193" alt="Splunk_logo" src="https://github.com/user-attachments/assets/9a2ab732-38cb-4f0b-808c-bb8bce0b8044" />

Splunk is a commercial Security Information and Event Management (SIEM) platform designed to collect, index, and analyze machine-generated data from IT systems, security devices, and applications in real time. It provides a centralized platform for monitoring, visualizing, and correlating logs, enabling security teams to quickly detect and respond to incidents.

Key features of Splunk include a powerful search processing language (SPL), customizable dashboards, real-time alerting, and advanced analytics capabilities. Its scalable architecture allows deployment in small, medium, or large enterprise environments, making it a versatile solution for organizations of varying sizes.

Splunk is particularly well-suited for environments where fast and actionable insights are critical, such as large-scale enterprises with complex IT infrastructures or organizations with dedicated Security Operations Centers (SOCs). Its strength lies in its extensive functionality, robust reporting capabilities, and support for a wide range of data sources.

**Key Features:**
- Powerful Search Processing Language (SPL)
- Customizable dashboards
- Real-time alerting
- Advanced analytics capabilities
- Extensive integration ecosystem (500+ apps)

---

## 4. ELK Stack Overview
![1_9sU-svzYO7aT7QdpnKmbBQ](https://github.com/user-attachments/assets/ef6c7f2e-c70d-4dcc-8735-3880dc083080)

The ELK Stack, consisting of Elasticsearch, Logstash, and Kibana, is an open-source SIEM and log management platform widely used for collecting, processing, and visualizing large volumes of machine-generated data. Elasticsearch provides a scalable search and analytics engine, Logstash handles data collection and transformation, and Kibana offers a visualization interface for dashboards and reporting.

Key features of the ELK Stack include advanced search capabilities, customizable dashboards, real-time log analysis, and flexibility for integration with various data sources. While highly powerful, the ELK Stack requires more setup and configuration compared to commercial solutions, and its learning curve can be steep for beginners.

The ELK Stack is particularly suitable for organizations that require highly customizable log analysis and visualization, such as engineering-focused environments or enterprises that need to process and analyze large datasets. Its open-source nature allows for cost-effective deployment, but it is best implemented by teams with experience in log management and system administration.

**Key Features:**
- Advanced search capabilities (Lucene, KQL, DSL)
- Customizable Kibana dashboards
- Real-time log analysis
- Flexible integration via Logstash and Beats
- Open-source with commercial cloud option (Elastic Cloud)

---

## 5. Graylog Overview
![Graylog-logo-blk](https://github.com/user-attachments/assets/cf375f53-1ff5-46b7-9fb9-01a197234602)

Graylog is an open-source SIEM platform designed for centralized log management, analysis, and monitoring. It collects and indexes data from multiple sources, providing security teams with a clear view of system events and potential threats in real time. Graylog emphasizes simplicity and ease of deployment while still offering powerful log correlation and alerting capabilities.

Key features include a user-friendly interface, built-in alerting, flexible dashboards, and support for a variety of input sources. While less complex than the ELK Stack, Graylog offers sufficient scalability for small to medium-sized environments and provides enterprise extensions for larger deployments.

Graylog is particularly suitable for organizations seeking a cost-effective and easy to manage SIEM solution, where fast deployment and simplicity are more critical than highly customizable features. Its intuitive interface and structured approach make it a practical choice for teams with limited resources or smaller SOCs.

**Key Features:**
- User-friendly web interface
- Built-in stream-based alerting
- Flexible dashboards
- Extractors for unstructured log data
- Content packs for common log sources

**Architecture Components:**
- Graylog Server (central node for log processing and alerting)
- Elasticsearch (backend storage and search engine)
- MongoDB (stores metadata, stream configurations, and user settings)

---

## 6. Hands-On Implementation

To conduct this evaluation, I worked with Splunk and ELK Stack through hands-on labs and academic training, supplemented by research and documentation analysis for Graylog.

### Lab Environment

| Component | Details |
|-----------|---------|
| **Platform** | TryHackMe (Splunk) / Academic Lab Environment (ELK Stack) |
| **Operating System** | Ubuntu 18.04 LTS |
| **Tools Deployed** | Splunk Enterprise, ELK Stack (Elasticsearch, Logstash, Kibana), TheHive |

### Splunk Implementation (TryHackMe)

Through guided lab exercises, I gained practical experience with Splunk's core functionality, including:

- **Navigation & Interface:** Explored the main Splunk dashboard, understanding the layout and available panels for security monitoring.
- **Data Ingestion:** Learned how to upload and classify logs, configuring sourcetypes to properly categorize different data sources.
- **Data Analysis:** Practiced searching and filtering logs using Splunk's Search Processing Language (SPL) to extract meaningful insights from machine data.
- **Visualization:** Created and customized different visualization types including graphs, tables, and charts to represent security data effectively.
- **Dashboard Exploration:** Reviewed and interacted with pre-configured dashboards to understand how Splunk presents security metrics and alerts.

### ELK Stack Implementation (Academic Environment)

My experience with ELK Stack extends beyond basic setup to full integration within a Security Operations workflow:

- **Deployment:** Installed and configured ELK Stack from scratch, establishing connections between Elasticsearch, Logstash, and Kibana for seamless log ingestion and analysis.
- **Log Source Integration:** Worked with multiple log sources including firewall logs, proxy logs, IDS alerts, Windows Event Logs, Linux system logs, and server logs — learning to parse and normalize data from diverse sources.
- **TheHive Integration:** Used ELK Stack in conjunction with TheHive as a ticketing system. When alerts are generated, I investigated alerts within Kibana dashboards, determined if alerts are true or false positives, and created/managed tickets in TheHive for incident tracking.
- **Incident Response Lifecycle:** Developed skills in the full incident response process including detection, analysis, containment and remediation, prevention, and postmortem reporting.

### Graylog Evaluation

Due to architectural similarities with ELK Stack (both utilize Elasticsearch as a backend), Graylog was evaluated through research, including review of official documentation, community resources, and feature comparisons.

**Key Technical Features of Graylog:**
- **Streams:** Logs are routed to different streams based on rules, allowing logical separation of data for targeted analysis and alerting.
- **Pipelines:** Processing rules enable log enrichment, field extraction, and normalization before data is stored.
- **Extractors:** Provide parsing capabilities for unstructured log data.
- **Alerting:** Stream-based alerting with support for HTTP callbacks, emails, or forwarding to external systems.
- **Content Packs:** Pre-packaged dashboards, streams, and extractors for common log sources.

**Verdict:** Graylog is well-suited for small to medium organizations seeking a cost-effective, easy-to-manage SIEM solution that balances functionality with operational simplicity.

---

## 7. Comparison of SIEM Solutions

| Feature | Splunk | ELK Stack | Graylog |
|---------|--------|-----------|---------|
| **License/Cost** | $$$ (commercial license) | Open Source (Free) / Elastic Cloud ($$) | Free / $$ (enterprise option) |
| **Deployment Complexity** | Medium | High | Low |
| **Ease of Use** | Medium (SPL required) | Hard (steep learning curve) | Easy (intuitive UI) |
| **Query Language** | SPL (Splunk Processing Language) | Lucene / KQL / DSL | Graylog Search Syntax |
| **Alerting** | Real-time saved searches | Watcher (Elasticsearch) | Stream-based alerts |
| **Visualization** | Highly customizable dashboards | Kibana (powerful but complex) | Built-in widgets, simpler |
| **Scalability** | High (horizontal scaling) | High (Elasticsearch native) | Medium (requires enterprise for large scale) |
| **Learning Curve** | Medium | High | Low |
| **Best For** | Large enterprises, dedicated SOCs | Engineering-focused teams, large datasets | SMBs, teams needing quick deployment |
| **Integration** | Extensive (500+ apps) | Flexible via Logstash/Beats | Good, but smaller ecosystem |

---

## 8. Real-World Case Study: Incident #147

To demonstrate how SIEM platforms enable effective incident response, I present a real investigation conducted in my academic SOC environment using ELK Stack and TheHive. This case illustrates the full incident response lifecycle, from initial detection through containment and reporting.

### Incident Overview

| Field | Details |
|-------|---------|
| **Date of Incident** | March 20, 2026 |
| **Source IP** | 10.10.2.21 |
| **Affected User** | p.rousseau |
| **Severity** | High |
| **ES Index** | soc-proxy-2026.03.20 |

### 1. Initial Detection

The incident was triggered by multiple correlated alerts across proxy, firewall, and IDS logs within ELK Stack:

- **Proxy Alert:** Download of `remotehelper.exe` (~9 MB) from `download-client-apps.net` — a remote administration tool commonly abused by attackers.
- **Web Server Log:** SQL injection attempt `GET /admin.php?id=1' OR '1'='1` targeting internal web server SRV-WEB.
- **IDS Alerts:** Detection of Nmap scanning, Wireshark traffic capture, and PsExec execution — all flagged as policy violations.

### 2. Investigation Process Using ELK Stack & TheHive

Using Kibana dashboards, I correlated logs across multiple sources to reconstruct the attack timeline:

| Timestamp | Log Source | Activity |
|-----------|------------|----------|
| 08:08:12 | Windows (Event ID 4740) | Account lockout for p.rousseau — early reconnaissance |
| 08:44:26 | Linux (SSH) | Successful SSH login to SRV-WEB using public key |
| 09:45:10 | Proxy | Download of remotehelper.exe |
| 09:46:10 | Web Server | SQL injection attempt on admin.php |
| 09:57:11 | Windows (Event ID 4688) | PsExec.exe execution — lateral movement |
| 09:58:41 | IDS | Putty.exe detected — SSH access attempt |
| 10:02:12 | Firewall | HTTP connection to internal web server — SQL injection tests |
| 10:10:12 | IDS | Nmap.exe detected — port scanning |

After verifying the alert as a **true positive**, I created a ticket in TheHive to document the incident and track the investigation.

### 3. Kill Chain Mapping

Using the Cyber Kill Chain framework, I mapped the attacker's progression:

| Phase | Observed Activity |
|-------|-------------------|
| **Reconnaissance** | Nmap scanning, Wireshark monitoring, account lockout attempts |
| **Weaponization** | Download of remotehelper.exe |
| **Delivery** | SSH connections to SRV-WEB and SRV-BDD |
| **Exploitation** | SQL injection `GET /admin.php?id=1' OR '1'='1` |
| **Lateral Movement** | PsExec execution on Windows host PC-DSI01 |
| **Obfuscation** | Use of legitimate-looking processes (WinWord.exe, PowerShell script) |

### 4. Containment & Remediation

Upon confirming the incident, I recommended and coordinated the following actions:

1. Isolate host 10.10.2.21 immediately to prevent further spread
2. Conduct forensic analysis on affected systems (SRV-WEB, SRV-BDD, PC-DSI01)
3. Review all administrative logins and tool executions
4. Implement network controls to block or monitor PsExec, Putty, Nmap, and Wireshark
5. Educate staff on risks of executing unknown tools or scripts

### 5. Postmortem Report

A full postmortem report was documented, including:

- Root cause analysis (attacker gained access via compromised credentials)
- Timeline of events with supporting log evidence
- Recommendations for preventing similar incidents (MFA enforcement, application whitelisting)

### Lessons Learned

This incident demonstrated the critical role of SIEM platforms in modern security operations:

- **ELK Stack** enabled rapid correlation of logs across disparate sources (proxy, firewall, IDS, Windows, Linux)
- **TheHive** provided structured case management, ensuring no investigation steps were missed
- The **Cyber Kill Chain** framework helped communicate the attack narrative clearly to stakeholders

This hands-on experience reinforced my ability to detect, investigate, and respond to real security incidents using SIEM tools in a production-like environment.

---

## 9. Use Cases

**Splunk:** Best suited for large enterprises with complex IT infrastructures and dedicated Security Operations Centers (SOCs). Its advanced analytics and reporting make it ideal for organizations that require fast, actionable insights.

**ELK Stack:** Ideal for engineering-focused teams or organizations that need highly customizable log analysis and visualization. Its open-source nature allows flexibility for large datasets, but it requires experienced teams for deployment and maintenance.

**Graylog:** A cost-effective solution for small to medium-sized organizations or teams with limited resources. Graylog emphasizes ease of use and quick deployment while providing sufficient functionality for effective log management and alerting.

---

## 10. Security Considerations

SIEM solutions play a crucial role in an organization's cybersecurity posture by providing real-time monitoring, threat detection, and alerting capabilities. Based on my hands-on experience with Splunk and ELK Stack, as well as my incident investigation work, I've identified the following key security considerations:

**Log Integrity:** Ensuring collected logs are complete, unaltered, and tamper-proof is essential for accurate incident detection and forensic analysis. During my investigation of Incident #147, I relied on timestamp consistency across proxy, firewall, IDS, and system logs to reconstruct the attack timeline. Any gaps or manipulation would have compromised the investigation.

**Detection Capabilities:** Each SIEM differs in correlation rules, alerting mechanisms, and threat intelligence integration. In my ELK Stack environment, I worked with pre-configured watchers that triggered on specific patterns (e.g., PsExec execution, Nmap scans). However, I found that fine-tuning these alerts was necessary to reduce false positives and ensure critical incidents weren't buried in noise.

**Access Control:** Proper configuration of user roles and permissions is necessary to prevent unauthorized access to sensitive logs and dashboards. In a SOC environment, this is particularly critical when handling incidents involving privileged accounts as seen in Incident #147 where user p.rousseau's credentials were compromised.

**Correlation Across Sources:** A SIEM's true value comes from its ability to correlate events across disparate log sources. During my incident investigation, I was able to connect proxy logs (tool download), Windows Event Logs (PsExec, Wireshark execution), IDS alerts (Nmap scanning), Linux auth logs (SSH access), and firewall logs (connection patterns). This cross-source correlation was essential for understanding the full attack chain.

**Scalability and Performance:** The ability to handle large volumes of log data without performance degradation is critical for maintaining effective security monitoring. In my academic environment, ELK Stack handled multiple concurrent data streams without noticeable latency, demonstrating its scalability for small to medium SOC operations.

**Compliance & Documentation:** SIEM platforms aid in meeting regulatory requirements (such as GDPR, ISO 27001) by providing audit trails, reports, and documentation. For Incident #147, the postmortem report I generated relied heavily on timestamped logs exported from ELK Stack, which would serve as evidence for compliance audits.

---

## 11. Conclusion

This comparative analysis of Splunk, ELK Stack, and Graylog demonstrates that each SIEM solution has unique strengths and is suited to different organizational needs.

| Solution | Best Suited For | Key Trade-Off |
|----------|----------------|---------------|
| **Splunk** | Large enterprises with dedicated SOCs | Powerful but expensive |
| **ELK Stack** | Engineering-focused teams, large datasets | Highly flexible but complex to maintain |
| **Graylog** | Small to medium organizations | Easy to deploy but less scalable |

My hands-on experience with Splunk through TryHackMe provided foundational knowledge in log ingestion, classification, and visualization using SPL. Working with ELK Stack in my academic environment integrated with TheHive as a ticketing system gave me practical exposure to the full incident response lifecycle. The investigation of Incident #147 demonstrated my ability to correlate logs across multiple sources, map attacks to the Cyber Kill Chain, and produce actionable postmortem reports.

This project reinforced that no single SIEM is universally "best" — the optimal choice depends on organizational context, team expertise, and budget. The hands-on experience gained has equipped me to evaluate, deploy, and operate SIEM solutions effectively in real-world security operations environments.

---

## 12. Project Summary for CV / Portfolio

**Project Title:** Comparative Analysis of SIEM Solutions (Splunk, ELK Stack, Graylog)

**Key Skills Demonstrated:**
- SIEM deployment and configuration
- Log ingestion and parsing from diverse sources (Windows, Linux, firewall, proxy, IDS)
- Alert creation and tuning (SPL, Watchers, Streams)
- Dashboard creation and data visualization
- Incident investigation and correlation across multiple log sources
- Cyber Kill Chain mapping
- Ticketing system integration (TheHive)
- Postmortem reporting and documentation

**Tools & Technologies Used:**
- Splunk Enterprise (TryHackMe lab)
- ELK Stack (Elasticsearch, Logstash, Kibana)
- Graylog (research-based evaluation)
- TheHive (ticketing and case management)
- Log sources: Windows Event Logs, Linux auth logs, Firewall logs, Proxy logs, IDS alerts, Web server logs

**Key Achievement:**
Successfully investigated a real security incident (Case #147) using ELK Stack and TheHive, correlating logs across 6+ sources, mapping the attack to the Cyber Kill Chain, and delivering a comprehensive postmortem report with actionable remediation steps.

---

*This project demonstrates practical skills in SIEM operations, incident response, and security monitoring applicable to real-world SOC environments.*
