# Post-Exploitation Roadmap

This repository documents, hands-on roadmap for **Post-Exploitation** in offensive security operations.  
It covers techniques, custom tooling, and practical development in **Bash**, **Python**, **C**, and **Go**.

---

## 📌 Table of Contents

1. [Environment Setup](#1-environment-setup)
2. [Host-Based Post-Exploitation](#2-host-based-post-exploitation)
3. [Credential Access & Abuse](#3-credential-access--abuse)
4. [Persistence Techniques](#4-persistence-techniques)
5. [Lateral Movement](#5-lateral-movement)
6. [Active Directory & Kerberos Abuse](#6-active-directory--kerberos-abuse)
7. [Defense Evasion](#7-defense-evasion)
8. [Data Exfiltration](#8-data-exfiltration)
9. [Custom Tool Development](#9-custom-tool-development)
10. [OPSEC & Cleanup](#10-opsec--cleanup)

---

## 1. Environment Setup

- AD Lab with multiple domains & forests (e.g., via pfsense, ESXi, or Terraform)
- C2 Setup: Sliver, Mythic, or custom C2
- Redirector + CDN infrastructure
- Python virtual environment & Go workspace

---

## 2. Host-Based Post-Exploitation

- Host Enumeration (users, groups, scheduled tasks)
- File/Process/Service inspection
- AV/EDR detection & response analysis
- PowerShell, Bash & Python one-liners
- Bash and Python post-exploitation scripts

---

## 3. Credential Access & Abuse

- LSASS dumping (with & without Mimikatz)
- SAM & SYSTEM hive parsing
- DPAPI secrets extraction
- Credential Manager abuse
- Credential theft in Python and Go
- Token impersonation (Python + Windows API)

---

## 4. Persistence Techniques

- Registry run keys / WMI / Scheduled tasks
- DLL Hijacking & Service abuse
- Go-based persistence agent
- Python script for autoload persistence
- C loader with shellcode & beacon callbacks

---

## 5. Lateral Movement

- Pass-the-Hash / Pass-the-Ticket
- PSExec, WinRM, RDP hijacking
- SMB & Named Pipe relays (Impacket)
- Lateral tools in Python
- Go-based PsExec-like binary

---

## 6. Active Directory & Kerberos Abuse

- BloodHound & SharpHound path analysis
- DCSync / DCShadow
- Kerberoasting with Python & Go
- AD ACL abuse automation
- Abusing AdminSDHolder & GPOs
- Ticket forging with Rubeus / Go

---

## 7. Defense Evasion

- AMSI Bypass (C & PowerShell)
- ETW patching
- Inline syscall injection (C)
- LOLBins (Living Off the Land Binaries)
- Obfuscation: Python/Go payload splitters
- Shellcode encryption loaders

---

## 8. Data Exfiltration

- DNS Tunneling (Python)
- Steganography (Python-based encoder)
- Exfil to Dropbox, Google Drive via API
- Archive + AES encryption
- Custom Go client for stealth exfil

---

## 9. Custom Tool Development

### 🔧 Python
- Host recon & enumeration scripts
- Credential dumpers
- Covert channels

### 🔧 C
- Shellcode loaders (PE injection, DLL injection)
- Custom stagers with inline syscalls
- AV/EDR evasion payloads

### 🔧 Go
- Cross-platform agents
- Custom HTTP/DNS C2 beacons
- Process injection with Go syscall wrappers

### 🔧 Bash
- Unix-based enumeration & persistence
- SSH agent hijacking

---

## 10. OPSEC & Cleanup

- Cleaning artifacts (prefetch, logs, registry)
- Disabling Defender logs temporarily
- Secure deletion of payloads
- OPSEC-safe beaconing
- Python & Go cleanup scripts

---

## 📚 References

- [MITRE ATT&CK - Post-Exploitation](https://attack.mitre.org/)
- [Youtube](https://www.youtube.com/@_JohnHammond)
- [Sliver Framework Docs](https://github.com/BishopFox/sliver)
- [Impacket](https://github.com/fortra/impacket)

---

## 🧠 Contribution

Pull requests are welcome for additional scripts, techniques, or tool enhancements.
