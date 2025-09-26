# 🔒 Task 4 — Windows Firewall Configuration

> Windows Firewall configuration task for blocking Telnet traffic (port 23), with exports and evidence.

## 📌 Objective
This project demonstrates configuring and testing Windows Firewall using PowerShell and `netsh`.  
The task focuses on blocking insecure Telnet traffic (port 23), verifying the rule, and restoring the firewall to its original state.


---

## ✅ Results
- Port **23/TCP (Telnet)** was successfully blocked.  
- Firewall configuration was exported as backup.  
- Rule was verified, tested, and then removed.  
- Evidence (screenshots & exports) included in this repo.  

---

## 📎 Files Included
- **commands.txt** → List of commands executed  
- **findings.md** → Short report with observations & conclusion  
- **evidence/** → Screenshots from each step  
- **exports/** → Firewall backup files (`.wfw`, `.xml`)
- **Summary/** → summary that how firewall filters traffic

---

## 📖 Key Notes
- Windows Firewall can be managed via both **PowerShell (`Get-NetFirewallRule`, `New-NetFirewallRule`)** and **`netsh`**.  
- Always **export/backup** firewall settings before changes.  
- Telnet (port 23) is blocked because it is insecure (transmits data unencrypted).  

