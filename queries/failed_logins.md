# Description: 
This query identifies failed Windows login attempts (`EventCode 4625`), grouped by user and host, and without groupping. 

# Grouped
index=main sourcetype=WinEventLog:Security EventCode=4625
| stats count by Account_Name, host

# Not Gouped
index=* sourcetype=WinEventLog:Security EventCode=4625

