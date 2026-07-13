# Metasploitable2 Penetration Testing Report (WIP)

## Overview
This repository contains a structured penetration test conducted against the Metasploitable2 vulnerable virtual machine. The objective was to identify, exploit, and analyse multiple misconfigured services and known backdoors.

## Scope
- FTP (21)
- IRC (6667)
- SMB (139/445)
- RPC / r-services (512–514)
- distccd (3632)
- Ingreslock (1524)

## 📌 Exploits Performed

1. [vsftpd 2.3.4 Backdoor (FTP 21)](01-vsftpd-backdoor/exploit-report.md)
2. [UnrealIRCd Backdoor (IRC 6667)](02-unrealircd-backdoor/exploit-report.md)
3. [Ingreslock Bind Shell (1524)](03-ingreslock-backdoor/exploit-report.md)
4. [distccd Remote Command Execution (3632)](04-distccd-exploit/exploit-report.md)
5. [Samba Symlink Traversal (139/445)](05-samba-symlink-traversal/exploit-report.md)
6. [r-services Trust Misconfiguration (512–514)](06-r-services-exploit/exploit-report.md)

## 📊 Summary Documents

- [Executive Summary](executive-summary.md)
- [Vulnerability Summary Table](vulnerability-summary.md)


## Tools Used
- Metasploit Framework
- smbclient
- telnet
- nmap

## Key Findings
Multiple critical vulnerabilities were identified, including:
- Remote backdoors allowing root access
- Unauthenticated service exploitation
- Misconfigured file-sharing services exposing the root filesystem

## ⚠️ Overall Risk Rating
CRITICAL

## Disclaimer
All testing was conducted in a controlled lab environment using intentionally vulnerable systems for educational purposes.

---

## Attribution
Metasploit VM is provided for educational use by Rapid7.
