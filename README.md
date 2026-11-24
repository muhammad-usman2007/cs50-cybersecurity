# CS50's Introduction to Cybersecurity

I completed this Harvard CS50 course in November 2026 as a 1st-year cybersecurity student.

![CS50 Certificate]

Verify my certificate: https://cs50.harvard.edu/certificates/59805932-ef5e-4794-b2d2-435a4e76d178

## What I learned

### Week 0: Securing Accounts
- Longer passwords are much harder to crack. Good practice is to check passwords against breached lists and not force regular changes.
- Multi-factor login combines something you know, something you have and something you are. App codes are safer than SMS codes, which can be stolen through SIM swapping.
- Phishing, credential stuffing and keylogging target people, so unique passwords, a password manager and not trusting email links matter most.

### Week 1: Securing Data
- Hashing turns data into a fixed-size code that cannot be reversed. Sites store the hash, not the password.
- Salting adds a random value before hashing, so the same password gives different hashes and cracking costs more.
- Public-key cryptography lets strangers share data securely. Digital signatures prove who sent a document.

### Week 2: Securing Systems
- Plain HTTP can be read or changed on the way. HTTPS uses TLS and certificates to protect traffic and prove a site's identity.
- VPNs encrypt traffic, SSH runs commands on remote servers securely, and firewalls filter traffic on ports.
- Malware includes viruses, worms and botnets. Updates and antivirus software reduce the risk, but zero-day attacks are still a danger.

### Week 3: Securing Software
- Injection attacks such as XSS, SQL injection and command injection happen when user input is trusted. Escaping input and using prepared statements prevent them.
- Checks that only run in the browser can be bypassed, so validation must also happen on the server.
- Bug bounties and CVE tracking help find and fix flaws, and signed software and trusted app stores help users avoid fake software.

### Week 4: Preserving Privacy
- Clearing history does not stop servers from logging visits. Fingerprinting can identify you from your browser details even without cookies.
- Cookies keep you logged in, while third-party cookies and tracking parameters follow you across sites.
- VPNs, encrypted DNS and Tor add privacy, but no tool gives absolute protection. Review app permissions regularly.

## Final project
A video report on **ToolShell**, a Microsoft SharePoint attack campaign from **July 2025**.
- CVEs: CVE-2025-49704, CVE-2025-49706, CVE-2025-53770, CVE-2025-53771
- Video (recorded November 8, 2026): https://www.youtube.com/watch?v=MLEoDU0eOlM
- What happened: In July 2025, attackers exploited flaws in on-premises Microsoft SharePoint Server. A crafted request to the ToolPane page skipped login checks and ran code on the server. Attackers planted web shells, stole the server's machine keys, and in some cases deployed ransomware. Microsoft linked the activity to the China-based groups Linen Typhoon, Violet Typhoon and Storm-2603. SharePoint Online was not affected.
- What would have prevented it: Installing Microsoft's patches quickly and completing every update step, keeping SharePoint servers off the open internet or behind a VPN or gateway, turning on AMSI and endpoint protection, and rotating the machine keys after patching.
- Course link: Week 3 (software flaws, patching and CVEs) and Week 2 (systems and malware).

Sources: [Microsoft Threat Intelligence](https://www.microsoft.com/en-us/security/blog/2025/07/22/disrupting-active-exploitation-of-on-premises-sharepoint-vulnerabilities/) and [Securelist: ToolShell explained](https://securelist.com/toolshell-explained/)

## What I'm doing next
Building hands-on skills with TryHackMe, aiming for SOC analyst roles.
