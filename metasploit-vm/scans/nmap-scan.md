## Target Identification

The `ifconfig` command was used to identify the IP address of the Metasploit VM.

**Result:**
- Target IP: 192.168.23.129

---

## Port Scanning

Nmap was used to scan the target machine and identify open ports and services.

## Command Used
```bash
nmap -sV -sC 192.168.23.129
```
## Findings
Multiple ports open due to intentionally vulnerable configuration
Services exposed for exploitation

## Analysis

The Metasploit VM is designed to be vulnerable, meaning exposed services are potential entry points for exploitation.
