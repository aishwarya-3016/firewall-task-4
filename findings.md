# Task 4 — Windows Firewall

## Objective
Configure Windows Firewall to block insecure Telnet traffic (port 23) and verify functionality.

## Steps
1. Listed existing rules using `Get-NetFirewallRule`.
2. Exported current firewall config (`netsh advfirewall export`, `Export-Clixml`).
3. Added inbound block rule for TCP/23 (`New-NetFirewallRule`).
4. Verified rule creation with PowerShell and `netsh`.
5. Tested using `Test-NetConnection` → connection to port 23 failed (expected).
6. Removed the rule using `Remove-NetFirewallRule`.

## Results
- Port 23 was successfully blocked.
- Firewall configuration exports saved in `/exports/`.
- Screenshots captured in `/evidence/`.

## Conclusion
Windows Firewall correctly enforced custom inbound rules. Blocking Telnet improves system security by preventing insecure, unencrypted connections.
