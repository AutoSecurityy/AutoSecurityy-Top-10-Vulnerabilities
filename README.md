# AutoSecurityy's Top 10 Automotive Cybersecurity Vulnerabilities
Draft - Accepting Pull Requests
---
No. | Vulnerability| Description
----|----|----
1|CAN Bus Injection via OBD-II or Exposed Lines|When vehicles lack authentication on CAN messages. Attackers can inject arbitrary frames via the OBD-II port or exposed in-vehicle wiring (e.g., behind lamps, infotainment units). This can lead to actions like unlocking doors, disabling braking systems, or spoofing sensor data.
2|Remote Keyless Entry System (RKES) Attacks|Relay attacks, roll-jamming (blocking signal during lock), replaying recorded signals, and exploiting key fob weaknesses can enable unauthorized vehicle entry or start — even without physical key access. This is widely used in real-world vehicle thefts.
3|Vulnerable API Endpoints in Connected Ecosystem|APIs exposed by mobile apps, telematics servers, or companion web apps often suffer from IDORs, poor session control, or token leakage. Exploiting these allows remote attackers to control vehicle functions (lock/unlock, start engine) or exfiltrate user data.
4|Weak Authentication & Authorization in UDS Services|Improper implementation of UDS protocols (e.g., 0x27 SecurityAccess or 0x10 Session Control) allows unauthorized users to gain extended diagnostic privileges, erase memory, or reprogram ECUs without valid credentials or challenge-response validation.
5|Insecure Wireless Interfaces (Bluetooth, Wi-Fi, TPMS, NFC)|Vehicles offer multiple wireless interfaces — often insecurely implemented. Weak pairing in Bluetooth, default Wi-Fi passwords, unencrypted TPMS signals, or NFC abuse can expose entry points for nearby attackers to inject commands or pivot deeper.
6|Inadequate Cryptographic Key Management|Hardcoded symmetric keys, key reuse across fleets, or poor entropy in key generation leaves systems open to reverse engineering or brute-force attacks. Lack of secure key storage or HSMs makes recovery and message spoofing easier for attackers.
7|Lack of Secure Boot & Firmware Validation|When ECUs boot unsigned or improperly verified firmware, attackers can inject malicious payloads that persist across reboots. Without chain-of-trust verification, even small ECUs become entry points for deeper compromise.
8|Insecure OTA Update Mechanism|Many vehicles lack strong protections for software updates. Weak hash validation, absence of rollback protection, or use of plain-text channels allows attackers to install tampered firmware or downgrade to known vulnerable versions.
9|Unprotected Debug Interfaces (UART, JTAG, SWD, etc.)|Exposed or unprotected low-level interfaces allow direct access to bootloaders, file systems, and runtime memory. Many ECUs ship with debug access left enabled, enabling firmware dumping, memory tampering, and bypassing protections.
10|No Logging, Monitoring, or Anomaly Detection|Vehicles typically lack runtime intrusion detection or event logging. This allows sophisticated attacks to run unnoticed, whether through internal message injection, unexpected firmware behavior, or OTA abuse.

## About the Project
As part of the AutoSecurityy community initiative, we are building a publicly available reference list inspired by the OWASP Top 10 — tailored specifically for automotive cybersecurity.

This list aims to highlight the most commonly exploited and impactful vulnerabilities found across modern vehicle platforms, based on hands-on experience, practical testing, and community input. We believe that with your experience and domain knowledge, your input would be incredibly valuable in refining this effort.
Contribute to the project by filling this form: https://forms.gle/cPXnAUQ3WBhmyZ14A


