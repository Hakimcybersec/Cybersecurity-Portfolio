# VSFTPD Backdoor Exploitation

## Description
The FTP service running on port 21 contains a known backdoor vulnerability.

---

## Vulnerability Details
- Service: vsftpd
- Backdoor triggered by username ending with: :)

---

## Exploitation

### Method 1: Manual (Telnet)
1. Connect to FTP service  
2. Enter malicious username  
3. Backdoor opens shell on port 6200  

### Method 2: Metasploit
Use the Metasploit module to automate exploitation.

---

## Outcome
- Remote shell access gained  
- Ability to execute commands  

---

## Impact
- Unauthorized access  
- Full system compromise  

---

## Remediation
- Update/remove vulnerable vsftpd version  
- Monitor unusual login patterns  
- Disable unnecessary services
