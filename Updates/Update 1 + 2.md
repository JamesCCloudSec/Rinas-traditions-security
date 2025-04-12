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
