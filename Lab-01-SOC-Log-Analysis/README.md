# SOC Log Analysis – Windows & Kali Linux

## Objective
To analyze authentication logs from Windows and Linux systems and identify failed login attempts as part of SOC Level-1 monitoring.

## Tools & Technologies
- Windows Event Viewer
- Kali Linux
- SSH
- journalctl
- grep, wc

## Lab Environment
- Windows system used for Event Viewer security log analysis
- Kali Linux used to generate and analyze SSH authentication logs
- Failed authentication attempts were generated intentionally for testing and analysis

## Windows Log Analysis
- Opened Windows Event Viewer
- Navigated to Windows Logs → Security
- Analyzed Event ID 4625 (Failed Logon)
- Observed details such as:
  - Username
  - Logon type
  - Timestamp
  - Failure reason

## Linux (Kali) Log Analysis
- Enabled SSH service on Kali Linux
- Generated failed SSH login attempts using invalid usernames
- Analyzed authentication logs using:
  - journalctl
  - grep for "Failed password"
- Counted failed login attempts to identify suspicious behavior

## Findings
- Windows Event ID 4625 indicates failed authentication attempts
- Linux SSH logs record failed login attempts with timestamps and usernames
- Multiple failed logins may indicate brute-force or unauthorized access attempts
- Log analysis is critical for early attack detection in SOC operations

## Skills Gained
- Windows security log analysis
- Linux authentication log analysis
- SOC Level-1 investigation workflow
- Understanding of authentication failure indicators

## Conclusion
This lab demonstrates practical experience in analyzing Windows and Linux authentication logs, a core responsibility of SOC analysts for detecting suspicious login activity.

