# Rinas's Traditions - Security Framework Development
**Start:** 03-25-2025
**Author:** James Castro
**Status:** In Progress | Volunteer Lead Security Engineer

## Overview:
This repository documents the security hardening and infrastructure planning I'm implementing for Rina's Traditions, a small business operating in-person and online.
I proposed and created the security role to provide professional-grade protections for the business while developing my personal hands-on experience across real-world systems.

## Objectives:
- Identify and mitigate key risks.
- Implement best practices in authentication, access, backups, and network posture.
- Build sustainable security processes that will scale as the business does.
- Develop reusable documentation, SOPs, and frameworks for business security.

## Environment:
- POS: Square
- Devices: iPhone, Windows Systems
- Accounts: Gmail, ****** Bank, Undisclosed Insurance Manager at Owner Request.
- Wi-Fi: Home + Restaurant, requires hardening.
- Website: Domain purchased, will help develop website.
- Authentication: PIN, FaceID, inconsistent 2FA/MFA
- Backup Strategy: None

## WIP:
- Reconnaissance
- Topology
- Documentation

## Roadmap (Next Few Months - Will Expand on Completion)
1. Threat Modeling
2. Credential Hygiene
3. MFA Implementation
4. Device Hardening
5. Network Hardening
6. Backup & Recovery
7. Vendor Security Audit
8. Monitor & Log
9. Website & Domain
10. Customer Data Protection
11. Business Continuity & Incident Response
12. Monthly Security Reports
13. Prepare for Growth and Expansion

## UPDATE #1 4/10/2025

**Toolkit Creation**

**/INSTALLERS/**
- 7-Zip
- Bitwarden
- Firefox
- Malwarebytes
- Nmap
- Notepad++
- SyncBackFree
- VeraCrypt
- VirtualBox (with Ubuntu ISO)
- Wireshark

**/DOCUMENTATION/**
- Logs and documentation organized by project

**/TRAINING/**
- Cheat Sheets
- Phishing awareness
- Security best practice
- Bitwarden guide

**/CONFIG/**
- Basic scripts for firewall, structure, and hardening stubs

**/BACKUP/**
- Organized for air-gapped backups and cloud backup staging

## UPDATE #2 — 2025-04-11

**Toolkit Expansion & Client Scheduling**

**Scheduled Security Implementation:**  
Sunday, April 13, 2025

**Note:** For ongoing toolkit changes after this update, see the dedicated [TOOLKIT GitHub Repository](https://github.com/JamesCCloudSec/field-security-toolkit) (link if hosted).

---

### /CONFIG/
- Initial creation of the `CONFIG` directory containing field-use scripts.

#### `Backup/`
- `create-backupfolders.ps1` — Script to generate clean backup folder structure
- `BACKUP_ORGANIZER.bat` — Bypass admin prompts with launcher
- `README.txt` — Purpose and usage documentation

#### `Bluetooth/`
- `DISABLE_BLUETOOTH.ps1`, `ENABLE_BLUETOOTH.ps1`
- Launchers: `DISABLE_LAUNCHER.bat`, `ENABLE_LAUNCHER.bat`
- `README.txt` — Registry-level Bluetooth control for public environments

#### `Firewall/`
- `DISABLE_LAN.ps1` — Blocks inbound LAN connections
- `UNDO_LAN.ps1` — Reverts changes
- Launchers: `DISABLE_LAN_LAUNCHER.bat`, `ENABLE_LAN_LAUNCHER.bat`
- `README.txt` — Explains use cases and limitations

#### `System/`
- `SYSTEM_REPORT.ps1` — Gathers system audit information
- `SYSTEM_REPORT_LAUNCHER.bat`

---

### /INSTALLERS/
- Added:
  - `Ventoy` — Multiboot ISO loader
  - `ProtonVPN` — Free secure VPN option for client or travel use

---

### /DOCS/
- Renamed structure and added three core categories:

#### `Operator Documents/`
- `Advanced Incident Response.docx` — Internal reference

#### `Rina's Traditions Documentation/`
- `CHECKLISTDAY1.docx` — Hardening, encryption, and backup implementation log

#### `Templates/`
- `Incident Response Form.docx`
- `Session Log Template.docx`

---

### /OPERATING SYSTEMS/
- Created `OPERATING SYSTEMS` folder for ISO use with Ventoy and VirtualBox

**ISOs Added:**
- Ubuntu
- Windows 10
- Windows 11
- Kali Linux
- ShredOS
- RescueZilla
- Hiren's BootCD PE
- GParted Live

---

### /TRAINING/
- Organized into 5 subfolders:
  - `APPLICATIONS`, `BACKUP`, `GENERAL SECURITY`, `PHISHING`, `THREAT RESPONSE`

**Additions:**
- `Bitwarden Guide` → APPLICATIONS
- `Backup Practices` & `Restore Point vs System Image` → BACKUP
- `Security Best Practices` → GENERAL SECURITY
- `Phishing Awareness`, `Teaching Guide`, `Google Phishing Test` → PHISHING
- `THREAT RESPONSE` — Empty placeholder

---

### /VAULT/
- Created encrypted VeraCrypt volume labeled `VAULT`  
  - Intended for storing critical logs, passwords, client archives, and sensitive backups.



