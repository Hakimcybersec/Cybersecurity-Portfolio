# Metasploit VM – Penetration Testing Lab

## Overview
This project documents a structured penetration testing lab conducted against Metasploit VM, a deliberately vulnerable environment.

The objective was to identify vulnerabilities, gain initial access, and explore exploitation and post-exploitation techniques in a controlled setting.

---

## Scope
- Target: Metasploit VM (local lab)
- Environment: Controlled / isolated
- Testing Type: Internal penetration testing

---

## Methodology
Full methodology documented here:  
→ [Methodology](./methodology.md)

---

## Key Areas


- [Nmap Scan Results](./scans/nmap-scan.md)
- [Backdoor Exploitation](./findings/vsftpd-backdoor.md)  
  ![Backdoor Exploit](./images/vsftpd-backdoor.png)  
  *Figure: Exploiting the vsftpd backdoor to gain initial access.*

- [Unix Basics & Remote Services](./findings/unix-r-services.md)  
  ![Unix Services](./images/unix-r-services.png)  
  *Figure: Enumeration and exploitation of Unix remote services.*

---

## Tools Used
- Metasploit Framework  
- Nmap  
- Kali Linux  
- Linux CLI  

---

## Disclaimer
All testing was conducted in a controlled lab environment using intentionally vulnerable systems for educational purposes.

---

## Attribution
Metasploit VM is provided for educational use by Rapid7.
