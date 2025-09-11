🛡️ Security Alert Monitoring & Incident Response using Splunk

📌 Project Overview

This project simulates the responsibilities of a Security Operations Center (SOC) analyst using Splunk. The objective was to analyze log data, detect suspicious activities, classify threats by severity, and simulate incident response procedures. The exercise provided practical, hands-on SOC analyst experience and built skills in log monitoring, threat detection, and incident escalation.

⚙️ Tools & Data

Splunk Enterprise (Free Trial)

SOC_Task2SampleLogs (Sample log dataset)

🛠️ Methodology

Uploaded and indexed log data into Splunk.

Executed SPL queries to detect anomalies and suspicious activities.

Investigated individual alerts in detail.

Classified threats by severity (Low, Medium, High).

Simulated incident response actions for medium- and high-severity alerts.

🚨 Alerts Identified
1. Multiple Failed Login Attempts (Medium Severity)

Description: High volume of failed logins from a single IP, indicative of brute-force activity.

Impact: Possible unauthorized access and privilege escalation.

Response: Raised an internal alert; monitored IP for escalation.

2. Suspicious Host Activity – Potential Compromise (High Severity)

Description: Host 203.0.113.77 showed login → file access → malware detection sequence.

Impact: Possible host compromise leading to malware spread.

Response: Classified as high-priority; escalated to Tier 2 SOC analysts.

3. Malware Detection Alerts (High Severity)

Description: SPL queries flagged ransomware, Trojans, worms, spyware, and rootkits from multiple IPs.

Impact: Large-scale compromise risk (data theft, ransomware, privilege escalation).

Response: Configured Splunk alerts; blocked malicious IPs; initiated scans.

4. Suspicious Internal Connection Attempt – Possible Lateral Movement (High Severity)

Description: User charlie attempted internal connection to host 10.0.0.5 after failed logins and malware alerts.

Impact: Possible lateral movement and deeper compromise.

Response: Disabled account; isolated host; escalated to IR team.

📊 Dashboard Summary

A Splunk dashboard was built with column charts to visualize malware activity across multiple hosts. This helped quickly identify the most impacted systems and prioritize response actions.
