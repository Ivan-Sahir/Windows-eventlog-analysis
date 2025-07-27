# Windows-eventlog-analysis

# Windows Event Log Analysis in Splunk

I made this project to practice using Splunk for collecting and analyzing Windows Event Logs to detect suspicious activity.
I simulated basic SOC analyst tasks such as detecting failed login attempts, privilege escalations, and suspicious process creation.

# Overview

- Set up Splunk on Windows
- Ingest native Windows logs (Security, System, Application)
- Detect suspicious activity using SPL
- Visualize login patterns and alerts in dashboards

# Tools Used

- Splunk Enterprise (Free tier)
- Windows 10

# Key Detections

| Use Case | SPL Query File |
|----------|----------------|
| Failed logins | `queries/failed_logins.spl` |
| Successful logins | `queries/successful_logins.spl` |
| Special Privileges Assigned at Logon | `queries/privilege_assigned.spl` |
| Process Created | `queries/process_creation.spl` |


# What I Learned

- How to ingest and explore Windows Event Logs in Splunk
- Writing SPL queries for real-world detections
- Visualizing time-based log patterns


