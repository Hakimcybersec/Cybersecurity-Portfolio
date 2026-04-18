# Executive Summary

This penetration test was conducted on the Metasploitable2 environment to assess system security and identify exploitable vulnerabilities.

---

## 📌 Key Exploits Performed

- [vsftpd 2.3.4 Backdoor](01-vsftpd-backdoor/exploit-report.md)
- [UnrealIRCd Backdoor](02-unrealircd-backdoor/exploit-report.md)
- [Ingreslock Bind Shell](03-ingreslock-backdoor/exploit-report.md)
- [distccd Misconfiguration](04-distccd-exploit/exploit-report.md)
- [Samba Symlink Traversal](05-samba-symlink-traversal/exploit-report.md)
- [r-services Trust Exploit](06-r-services-exploit/exploit-report.md)

---

## 🔥 Overall Findings
The system contains multiple critical vulnerabilities allowing:
- Remote root-level access
- Unauthorized file system exposure
- Unauthenticated command execution

---

## ⚠️ Risk Rating
CRITICAL

---

## 📊 Detailed Breakdown
See: [Vulnerability Summary](vulnerability-summary.md)

## Recommendation
Immediate remediation of all exposed services, removal of backdoors, and strict access control enforcement.
