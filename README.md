# VirtuHost (Windows Server Lab)

VirtuHost is a hands-on Windows Server lab that simulates a small enterprise Active Directory environment.  
The goal is to practice and document real-world Windows administration: identity, policy, file services, access control, replication, and auditing.

This repo contains my configuration notes, screenshots, troubleshooting fixes, and PowerShell scripts used to build the environment.

---

## Highlights
- Active Directory Domain Services (AD DS) with structured OUs and group-based access
- DNS + DHCP
- Group Policy (GPO): drive mappings, policies, delegation and targeting
- File services: NTFS + share permissions, HomeDrive setup, Access-Based Enumeration (ABE)
- DFS Namespace + DFS Replication
- Auditing (Access Logs / Event-based tracking)
- PowerShell scripts for automation (users, groups, OUs, mappings, permissions)
- Troubleshooting log and validation screenshots (gpresult, access tests, etc.)

---

## Repo structure (how to navigate)
- **/Documentation/**  
  All topic-based documentation and proof screenshots (ABE, DFS, Auditing, NTFS, HomeDrive, etc.)
- **/Powershell script/**  
  PowerShell commands/scripts used for creation and configuration (users, groups, OUs, GPO mappings, permissions)
- **/Windows Srvs/**  
  Server-specific folders (DC-01, DC-02) and related configuration material
- **/FW/**  
  Firewall-related notes/screenshots
- **/Windows Server Installation files/**  
  Installation material used during setup
- **/usr background picture/**  
  Assets used for user environment customization
- **Excel/Word files**  
  Tables and reports used for structure and documentation (Drive mapping, identity table, report)

---

## Environment (high level)
- **Servers:** DC-01, DC-02 (Windows Server)
- **Core services:** AD DS, DNS, DHCP, GPO, File Services, DFS
- **Client support:** Windows 10/11 style endpoint management concepts (policies, mappings, permissions)

> Note: This is a lab project designed to mirror production concepts and best practices.

---

## Documentation index (quick links)
Inside **/Documentation/** you will find topics such as:
- **ABE/** (Access-Based Enumeration)
- **Auditing (Access Logs)/**
- **DFS/**
- **Disk Quotas/**
- **Domain Locals/**
- **Drive map item level targeting/**
- **Folder Redirection/**
- **HomeDrive/**
- **NTFS Permission/**
- **Topologi/** (diagrams / topology)
- **User Result drivers/** (validation output)

---

## PowerShell automation
Scripts are located in **/Powershell script/** and include:
- Create OUs / Users / Groups
- Nesting Global Groups into Domain Local Groups
- Drive mappings via GPO Preferences
- HomeDrive + NTFS permission setup
- Cleanup scripts (remove members, fix permissions, etc.)

---

## Why this project
VirtuHost was built to refresh and prove practical Windows Server / infrastructure skills through a documented and repeatable lab setup, including real troubleshooting and validated results.

---

## Status
Ongoing / improving documentation (README + topic documents are being expanded).
