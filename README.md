# splunk-ad-detection-lab
Splunk detection engineering lab - 20 MITRE ATT&amp;CK detections validated against Atomic Red Team on Windows Server 2022
# Splunk AD Detection Engineering Lab

Detection engineering project simulating 20 MITRE ATT&CK techniques using Atomic Red Team on Windows Server 2022, with Splunk SPL detections validated against ground-truth results.

## Stack
- **SIEM:** Splunk Enterprise 10.4.2 (Ubuntu 24.04)
- **Telemetry:** Sysmon 15 + Windows Security + PowerShell logs
- **Simulation:** Atomic Red Team
- **Forwarding:** Splunk Universal Forwarder 9.2.1
- **Lab OS:** Windows Server 2022 Standard Evaluation

## Coverage: 20/20 Techniques Detected

| ID | Technique | Tactic | Status |
|---|---|---|---|
| T1059.001 | PowerShell Encoded Command | Execution | ✅ |
| T1059.001 | PowerShell Download Cradle | Execution | ✅ |
| T1003.001 | LSASS Process Access | Credential Access | ✅ |
| T1003.002 | SAM Registry Dump | Credential Access | ✅ |
| T1053.005 | Scheduled Task Persistence | Persistence | ✅ |
| T1547.001 | Registry Run Key | Persistence | ✅ |
| T1110.003 | Password Spraying | Credential Access | ✅ |
| T1070.001 | Event Log Cleared | Defense Evasion | ✅ |
| T1218.011 | Rundll32 LOLBin | Defense Evasion | ✅ |
| T1218.005 | mshta.exe Remote Script | Defense Evasion | ✅ |
| T1136.001 | New Local Admin Account | Persistence | ✅ |
| T1087.002 | Domain Account Enumeration | Discovery | ✅ |
| T1047 | WMI Command Execution | Execution | ✅ |
| T1562.001 | Windows Defender Disabled | Defense Evasion | ✅ |
| T1562.002 | Audit Policy Disabled | Defense Evasion | ✅ |
| T1105 | certutil Downloader | Command & Control | ✅ |
| T1036.003 | Process Masquerading | Defense Evasion | ✅ |
| T1003.003 | Shadow Copy Abuse | Credential Access | ✅ |
| T1059 | Suspicious Parent-Child Process | Execution | ✅ |
| T1036 | Suspicious Executable in Temp | Defense Evasion | ✅ |
