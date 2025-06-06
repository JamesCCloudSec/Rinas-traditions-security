# Phase Two Deployment – Business Laptop Hardening  
**Client:** Rina’s Traditions  
**Date:** April 13, 2025  
**Technician:** James Castro  
**Follow-up:** April 15, 2025

Performed a complete security deployment of the business-only laptop for Rina’s Traditions **(see [Phase 2: Laptop in Update3_Checklist_Schedule](./Update3_Checklist_Schedule.md)).** This stage focused on secure device segmentation, separating personal usage from business usage, user role enforcement, encryption, credential management, and foundational hardening to support long-term business resilience.

## Scope & Context
This document summarizes the live security implementation of Phase Two from the Rina’s Traditions internal security plan, focused on the hardening of a business-exclusive laptop used for communications, vendor interactions, financial management, and authentication. The objective was to fully segment business operations from personal activity, enforce least privilege across user accounts, and deploy layered endpoint protections using free and licensed tools. This effort is part of a broader multi-phase deployment to elevate the business’s cybersecurity maturity with minimal cost and maximum transparency, aligning with NIST and FCC small business security guidance.
## Completed Tasks

### System Segmentation & User Role Enforcement
- Performed a full factory reset of the device
- Created two local accounts:
  - Admin (local) for elevated control
  - EthanWork (standard:local) for daily business use
- Enforced least privilege model: Ethan must use the admin account for all elevated actions; strongly advised against casual use

### Credential Security & Authentication
- Installed and configured Bitwarden password manager
  - Helped Ethan create a complex but memorable master password
  - Replaced all critical service credentials with complex, long, Bitwarden-generated passwords.
  - Migrated 5–6 business-critical logins (Gmail, Square, Instagram, Umpqua, Bitwarden, Admin)
  - Enabled and configured Google Authenticator for all services
  - Separated personal vs work authentication tokens
  - Performed hands-on training with supervised vault usage

### Encryption & Secure File Handling
- Installed VeraCrypt and created an encrypted file-based vault for sensitive business data (recipes, financial docs)
- Recovery key securely stored in Bitwarden

### Endpoint Protection & Threat Defense
- Removed Norton 360, which had hijacked firewall control
- Verified Windows Defender and Firewall were enabled and functional
- Installed Malwarebytes for layered threat detection
- Hardened Firefox:
  - Disabled auto-fill
  - Installed uBlock Origin for content and ad filtering

### Software Cleanup & Optimization
- Removed over 30 preinstalled bloatware applications and services
- Ensured only essential apps (Firefox, Bitwarden, Microsoft Office) remained

### Secure Connectivity
- Installed and configured ProtonVPN to support secure remote access

### Client Education & Access Policy
- Trained Ethan on Bitwarden, password security, role separation, and system update behavior
- Enforced "admin-for-critical-use-only" policy with clear login separation
- Confirmed client understanding and alignment with operational expectations

### Virtualization & Open-Source Training
- Installed VirtualBox and configured Ubuntu virtual machine environment
- Taught Ethan how to launch, use, and safely experiment with Ubuntu for learning purposes

## Resume Highlights – Phase Two Implementation (Rina’s Traditions)

- Deployed hardened local user architecture with strict least-privilege access controls and full admin segmentation
- Built secure identity stack using Bitwarden + Google Authenticator with unique, complex credentials and enforced 2FA across all business services
- Implemented secure file encryption using VeraCrypt with vault recovery key stored in a managed password vault
- Configured layered endpoint protection, including Windows Defender, firewall tuning, and Malwarebytes
- Eliminated over 30 preinstalled applications, optimizing system performance and reducing attack surface
- Resolved critical system conflicts including Norton 360 firewall hijacking and Microsoft account enforcement during device setup
- Installed and configured ProtonVPN to provide secure, encrypted remote access capability
- Delivered client training on password management, device roles, safe browsing, and VPN use
- Introduced open-source Linux training via VirtualBox and Ubuntu VM walkthrough

## Notes & Observations

- Encountered and resolved forced Microsoft login issue during setup
- Removed legacy firewall interference from Norton 360 and ensured Defender was re-enabled
- Laptop is now fully segmented, protected, and hardened for real-world business use
- All elevated actions require admin login; standard user account configured for daily operations
- Client follow-up scheduled for Tuesday, April 15, 2025, to complete Phases 1, 3, 4, 5, and 6 (Phase 2 completed today).
- Phase 1 was postponed due to a hardware malfunction. Ethan's backup device failed to move 1GB of critical data, requiring me to handle it on arrival.
