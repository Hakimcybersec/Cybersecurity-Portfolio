# UNIX R-Services Exploitation

## Description
The target system exposes legacy “r” services on TCP ports:
- 512 (rexec)
- 513 (rlogin)
- 514 (rsh)

These services are misconfigured and allow remote access without proper authentication.

---

## Approach
- Identified open r-services via scanning
- Attempted remote access using `rsh-client`

## Requirements
- Attacker must have `rsh-client` installed
- Root privileges required on attacking machine

---

## Exploitation
Access was attempted using remote shell commands due to weak authentication.

---

## Impact
- Unauthorized remote access  
- Potential full system compromise  

---

## Notes
If SSH keys are requested instead, it indicates `rsh-client` is not installed and SSH is being used instead.

---

## Remediation
- Disable r-services  
- Replace with secure protocols (SSH)  
- Restrict remote access
