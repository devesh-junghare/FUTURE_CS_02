# FUTURE_CS_02
# Security Operations Center (SOC) Internship Task 2 – Security Alert Monitoring & Incident Response Simulation

## Overview
This project simulates core activities of a Security Operations Center (SOC). The main goal is to **monitor security alerts, analyze potential threats, and simulate incident response**, just like a SOC analyst in a real-world environment. This repository contains all the resources, analysis, and reports generated during the internship task.

## Key Objectives
- Set up and explore **Splunk Enterprise 10.0.0** for log analysis.
- Analyze simulated security alerts and logs.
- Identify suspicious activities such as failed logins, unusual IP addresses, malware alerts, and unauthorized file access.
- Categorize and prioritize alerts based on severity.
- Draft a detailed **incident response report** with timeline, impact, and remediation suggestions.
- Simulate communication with stakeholders about incidents.

## Tools Used
- **Splunk Enterprise 10.0.0** – SIEM platform for ingesting, analyzing, and visualizing logs.
- **Sample Logs** – Provided by Future Interns for analysis.
- **Google Docs / MS Word** – For drafting incident response reports.

## Features Implemented
- **Log Analysis**: Categorized logs into login attempts, connection attempts, file access events, and malware alerts.
- **Identification of Suspicious Alerts**: Highlighted 3–5 high-priority alerts with detailed analysis.
- **Incident Classification**: Alerts were classified into **High, Medium, and Low** priority.
- **Detailed Incident Response**: Created timelines, assessed impact, and suggested remediation steps.
- **Dashboard Visualization**: Used Splunk dashboards to visualize failed logins, malware detections, and other security events.
- **Playbooks**: Explained standardized responses to incidents like brute-force attacks and malware infections.
- **Optional Communication Template**: Prepared an email draft reporting incidents to management.

## Suspicious Alerts Identified
| Timestamp           | User    | IP           | Action           | Threat                    | Priority |
|--------------------|---------|-------------|-----------------|---------------------------|----------|
| 2025-07-03 05:48:14 | bob     | 10.0.0.5    | malware detected | Trojan Detected           | High     |
| 2025-07-03 04:19:14 | alice   | 198.51.100.42 | malware detected | Rootkit Signature         | High     |
| 2025-07-03 05:06:14 | bob     | 203.0.113.77 | malware detected | Worm Infection Attempt    | High     |
| 2025-07-03 07:45:14 | charlie | 172.16.0.3  | malware detected | Trojan Detected           | High     |
| 2025-07-03 07:02:14 | alice   | 203.0.113.77 | login failed     | -                         | Medium   |

## Incident Response Highlights
- **Brute-force login attempts** were mitigated with account lockout policies and firewall restrictions.
- **Malware detections** were addressed through anti-virus solutions, endpoint monitoring, and user awareness training.
- **Unauthorized file access** prompted monitoring of exposed data and account restrictions.
- **Successful unauthorized logins** highlighted the need for multi-factor authentication and CAPTCHA implementation.
- **Lateral movement attempts** within the network were addressed by network segmentation and internal traffic monitoring.
