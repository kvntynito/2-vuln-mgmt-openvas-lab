# <Project Title>

This project demonstrates hands-on vulnerability management using Nmap and OpenVAS/GVM.
It includes scan outputs, analysis reports, risk matrices, and remediation planning based on real test environments.

## 🎯 Objectives
- Nmap scans
- OpenVAS reports
- Vulnerability Assessment template
- Risk Matrix

## 📁 What’s Inside
- `docs/` – reports, playbooks, baselines, diagrams
- `scripts/` – Python/PowerShell/Bash utilities
- `lab/` – sample logs, datasets, IaC
- `.github/` – issue/PR templates

## 🧪 Lab Setup (Quick Start)
A simple, reproducible home lab was used to perform scans:
- **Host:** Proxmox, VMware, Hyper-V, or VirtualBox
- **Targets:**
  - Metasploitable2
  - DVWA / WebGoat
  - Windows Server 2019 (unpatched)
  - Ubuntu Server with outdated packages
- **Network:**
  - VLANs or isolated “Security Testing” network
  - pfSense/OPNsense for segmentation

OpenVAS (GVM) was installed on Ubuntu Server, and Nmap was run from both Kali and Windows.

## ▶️ How to Run
**1. Run Nmap enumeration**
    - Upload your results into the lab/ folder.

**2. Run OpenVAS full scan**
Steps:

     1st - Launch GVM web console

     2nd - Create new Full and Fast task

     3rd - Add target IP(s)

     4th - Run scan

     5th - Export results as: PDF / CSV / XML

Upload exported files to the lab/ folder.

**3. Perform vulnerability analysis**
Populate:
- docs/Vulnerability_Assessment_TEMPLATE.md
- docs/Risk_Matrix_TEMPLATE.csv

Use CVSS scores, descriptions, and recommended remediation from the scanner.

## 📊 Deliverables
✅ Nmap scans

✅ GVM/OpenVAS vulnerability reports

✅ Risk Matrix with likelihood/impact scoring

✅ Standardized vulnerability assessment report

✅ Network diagram (optional but recommended)

✅ Screenshots of findings

✅ Remediation plan

## 🧠 What I Learned
- Bullet points of concepts/skills you gained - Write what you learned about scanning, false positives, CVSS.
- How to enumerate systems using Nmap
- How to run authenticated/unauthenticated scans
- How to interpret vulnerability findings vs. false positives
- Understanding CVSS scoring and risk prioritization
- Mapping vulnerabilities to remediation steps
- The workflow of a real vulnerability management program
- How to document findings clearly for stakeholders

## ✅ Next Steps
- Add authenticated scans (SSH or WinRM)
- Expand testing to cloud-hosted assets
- Add a script to automatically parse Nmap results
- Add a Python tool to correlate vulnerabilities with MITRE ATT&CK
- Perform regression scanning after hardening steps
- Add a summary dashboard (Grafana or Excel-based)

## ⚖️ License
MIT – see `LICENSE`.
