# Metasploit2 VM – Penetration Testing Lab Report

# Metasploitable2 Penetration Testing Report

## Overview
This repository contains a structured penetration test conducted against the Metasploitable2 vulnerable virtual machine. The objective was to identify, exploit, and analyse multiple misconfigured services and known backdoors.

## Scope
- FTP (21)
- IRC (6667)
- SMB (139/445)
- RPC / r-services (512–514)
- distccd (3632)
- Ingreslock (1524)

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

## Summary
Refer to `vulnerability-summary.md` for full impact analysis.
---

## Disclaimer
All testing was conducted in a controlled lab environment using intentionally vulnerable systems for educational purposes.

---

## Attribution
Metasploit VM is provided for educational use by Rapid7.
