## UPDATE — Rina’s Traditions Security Plan (Scheduled: 2025-04-13)

**Technician:** James Castro  
**Client:** Ethan (Owner, Rina’s Traditions)  
**Systems:** Desktop (Personal Use) + Work Laptop (Business Use)  

This update outlines the full scope of the security implementation scheduled for April 13, 2025. Tasks reflect hardening, backup readiness, authentication upgrades, encrypted storage setup, and live client training using my personal field toolkit.

---

### Group 1 — Desktop (Personal Use)

- Factory reset and clean system base
- Admin and standard user accounts created for privilege separation
- Strong password policy enforced
- Windows updates, Defender, and Firewall enabled
- 5-minute auto-lock and login-on-wake set
- VirtualBox installed; Ubuntu ISO provided (per client request)
- Personal apps reinstalled: Discord, Steam, Spotify, Curseforge
- Clear browser and account separation between work and personal profiles
- Restore point created
- Bluetooth disabled using field script
- VM risks explained (bridging, clipboard, host compromise)

---

### Group 2 — Laptop (Work-Only System)

- Factory reset
- Admin and standard user accounts created
- Strong, unique passwords generated via Bitwarden
- System fully updated with Windows Defender + Firewall enabled
- Auto-lock and session control configured
- Create partition with encryption via BitLocker or VeraCrypt (based on support)
- Firefox installed (work use only)
- Bitwarden installed on laptop + mobile
- Google Authenticator configured on mobile
- 2FA enforced on:
  - Gmail  
  - Instagram  
  - Square  
  - Bitwarden (biometric + token)  
- Square dashboard shortcut added to desktop
- Bloatware removed
- System restore point created
- Password vault organized by category
- MFA tested across accounts

---

### Group 3 — Backup Foundations

- Critical business files (recipes, financials, credentials) identified
- Triple backup system planned:
  - Physical flash drive
  - Work laptop (separate partition or encrypted vault)
  - Cloud backup (encrypted)
- Zip archive created for sensitive files
- Bitwarden vault attachments tested (free tier)
- SyncBackFree backup job configured and tested
- Client trained on how to perform manual and structured backups
- Backup folder system created and labeled

---

### Group 4 — Security Scripts & Hardening

- LAN traffic disabled via `DISABLE_LAN.ps1`
- Reversal tested with `UNDO_LAN.ps1`
- Bluetooth disabled via registry and PnP script
- Controlled Folder Access enabled to protect key directories
- Custom firewall rules reviewed and confirmed
- Restore point created post-hardening
- Offsite copies of sensitive files stored securely

---

### Group 5 — Client Training

- Phishing training delivered (concepts, detection, response)
- Bitwarden tutorial (browser extension, password strategy)
- Standard vs. Admin account responsibilities explained
- Manual backup and cloud/archive strategies covered
- Toolkit folders explained: `/TRAINING/`, `/SCRIPTS/`, `/DOCS/`
- Trained on handling phishing, password leaks, incident response

---

### Group 6 — System Imaging & Final Review

- System image created using RescueZilla (external drive)
- Drive labeled and secured offsite
- Advised Ethan not to modify system without guidance
- Final review confirmed backups, authentication, hardening
- Client documentation saved to:  
  `C:\Users\Ethan\Documents\Security_Overview\DayOne_Report.txt`

---
**For Future Document Use:**
### SIGN-OFF (To be completed on site)

- [ ] Client confirms understanding of account usage and recovery  
- [ ] MFA confirmed and working across all services  
- [ ] Scripts and automation tools demonstrated  
- [ ] Client walked through next steps post-deployment  
- [ ] Logs saved to `/DOCS/Rinas Traditions/`

---

**Date Started:** _(to be filled)_  
**Date Completed:** _(to be filled)_  

**Client Signature:** _____________________  
**Operator Signature:** ___________________
