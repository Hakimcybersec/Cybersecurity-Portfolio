# Metasploit VM – Penetration Testing Lab Report

🔹 Overview
Target: Metasploitable2 vulnerable VM
Objective: Identify and exploit misconfigured services and backdoors
Tools: Metasploit, smbclient, telnet, nmap

🔹 Scope of Testing
FTP (21)
IRC (6667)
SMB (139/445)
RPC / r-services (512–514)
distccd (3632)
Ingreslock (1524)

🔹 Summary Table

| # | Vulnerability                     | Service / Port | Exploit Type                 | Access Level      | Severity | Outcome                                             |
| - | --------------------------------- | -------------- | ---------------------------- | ----------------- | -------- | --------------------------------------------------- |
| 1 | vsftpd 2.3.4 Backdoor             | FTP / 21       | Malicious backdoor trigger   | Root              | Critical | Direct root shell via backdoor                      |
| 2 | UnrealIRCd 3.2.8.1 Backdoor       | IRC / 6667     | Metasploit backdoor exploit  | Root              | Critical | Reverse shell with root privileges                  |
| 3 | Ingreslock Backdoor               | 1524           | Direct telnet bind shell     | Root              | Critical | Immediate unauthenticated root access               |
| 4 | distccd Misconfiguration          | 3632           | Remote command execution     | Daemon            | High     | Low-priv shell, misconfiguration allows file access |
| 5 | Samba Symlink Traversal           | SMB / 139,445  | Filesystem traversal exploit | N/A (file access) | High     | Full filesystem read via SMB                        |
| 6 | r-services Trust Misconfiguration | 512/513/514    | Remote login trust abuse     | Root              | Critical | Remote root login via rsh/rlogin                    |

🔹 Key Skills Demonstrated
Network enumeration
Exploitation of known backdoors
Misconfiguration abuse
Privilege escalation analysis
File system traversal attacks

---

## Disclaimer
All testing was conducted in a controlled lab environment using intentionally vulnerable systems for educational purposes.

---

## Attribution
Metasploit VM is provided for educational use by Rapid7.
