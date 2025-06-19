# Splunk Windows Log Analysis

## Project Overview
This project demonstrates how to ingest and analyze Windows event logs using Splunk. As a cybersecurity recent graduate, gaining hands-on experience with log management and analysis tools like Splunk is critical to understanding system security, monitoring, and incident response.

## What is Splunk?
Splunk is a powerful platform used for searching, monitoring, and analyzing machine-generated data via a web-style interface. It is widely used in cybersecurity to gain insights from logs, detect threats, and improve security posture.

## Project Details
- **Logs used:** Windows Event Logs exported as CSV and sample log files.
- **Data ingestion:** Logs were uploaded to Splunk’s web interface and indexed with appropriate source types.
- **Analysis:** Basic searches were performed to filter by Event IDs and identify notable events such as service changes, login attempts, and errors.

## Why this matters
Windows event logs contain valuable information about system activities and security events. Analyzing these logs helps cybersecurity professionals detect suspicious activities, troubleshoot issues, and comply with security policies.

## How to run
1. Export Windows event logs to CSV format (or use sample log files).
2. Upload logs to Splunk via the Data Inputs page.
3. Set source type to `csv` or a relevant type.
4. Run Splunk search queries, e.g., `index=main source="sample_log.txt" EventCode=7040`.

## Sample Searches
```splunk
index=main source="sample_log.txt" EventCode=7040
index=main source="security_log.csv" EventID=1038
