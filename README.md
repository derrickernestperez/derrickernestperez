<div align="center">

# Derrick Ernest Perez

### Systems Administration • Infrastructure Operations • Identity and Access Management

Computer Science student building a hands-on Microsoft infrastructure homelab focused on Windows Server, Active Directory, PowerShell automation, enterprise troubleshooting, and technical documentation.

<br>

<a href="https://github.com/derrickernestperez/IT-Operations-Homelab">
  <img src="https://img.shields.io/badge/View%20the%20Homelab-0078D4?style=for-the-badge&logo=github&logoColor=white" alt="View IT Operations Homelab">
</a>

<a href="https://www.linkedin.com/in/derrickperez2002/">
  <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
</a>

<br><br>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=18&duration=2800&pause=900&color=0078D4&center=true&vCenter=true&width=900&lines=Windows+Server+Administration;Active+Directory+and+Group+Policy;DNS%2C+DHCP%2C+File+and+Print+Services;PowerShell+Automation;Infrastructure+Troubleshooting;Security+Monitoring+and+Documentation" alt="Technical focus areas">

</div>

---

## About Me

I am a Computer Science student developing practical experience in systems administration and enterprise IT operations.

My main project is a Microsoft-based homelab that recreates common responsibilities handled by Help Desk technicians, systems administrators, infrastructure engineers, and identity administrators.

I use the lab to practice more than installation. Each module includes configuration, validation, troubleshooting, automation, and documentation.

My current focus includes:

- Windows Server administration
- Active Directory and Group Policy
- Identity lifecycle management
- DNS and DHCP
- File and print services
- PowerShell automation
- Windows Admin Center
- Security monitoring
- Backup and recovery
- Microsoft cloud identity

---

## Featured Project

### [IT Operations Homelab](https://github.com/derrickernestperez/IT-Operations-Homelab)

A structured Windows enterprise environment built to practice infrastructure deployment, identity administration, endpoint management, troubleshooting, security monitoring, and operational documentation.

The repository is organized into the following areas:

```text
00-Lab-Setup
01-Identity-and-Access-Management
02-Core-Infrastructure
03-Enterprise-Operations
04-Cloud-Identity-and-M365
05-Security-Operations
06-GRC-and-Compliance
```

Each completed module documents:

- The business problem
- Why the technology is used
- The lab environment
- Implementation steps
- Screenshots and evidence
- Validation results
- Troubleshooting notes
- Security considerations
- Useful commands
- Interview preparation
- Personal lessons learned

---

## Homelab Architecture

```text
                         Internet
                            │
                  VMware Workstation Pro
                            │
                     Isolated Lab Network
                            │
          ┌─────────────────┴─────────────────┐
          │                                   │
        SRV01                              CLIENT01
 Windows Server 2025                  Windows 11 Enterprise
          │                                   │
          ├── Active Directory                ├── Domain joined
          ├── DNS                             ├── Group Policy managed
          ├── DHCP                            ├── Mapped drives
          ├── Group Policy                    ├── Folder Redirection
          ├── File Services                   ├── Deployed printer
          ├── Print Services                  └── Enterprise authentication
          ├── Windows LAPS
          ├── Windows Admin Center
          ├── PowerShell Automation
          └── Backup and Recovery
```

This is currently a single-server learning environment. Future phases will separate infrastructure roles across additional servers and introduce cloud identity, centralized monitoring, and security operations tooling.

---

## Current Environment

| Component | Current Configuration |
|---|---|
| Hypervisor | VMware Workstation Pro |
| Server | Windows Server 2025 |
| Client | Windows 11 Enterprise |
| Domain | `homelab.local` |
| Domain Controller | SRV01 |
| Managed Client | CLIENT01 |
| Active Directory Users | 20+ test accounts |
| Organizational Units | Department and infrastructure OUs |
| Security Groups | Department and access groups |
| Automation | PowerShell |
| Management | Server Manager and Windows Admin Center |
| Documentation | Markdown, screenshots, scripts, and reports |

The environment continues to grow as new modules are completed.

---

## Completed Work

### Identity and Access Management

- Active Directory Domain Services deployment
- Organizational Unit design
- User and security-group administration
- Windows 11 domain join
- Group Policy hardening
- Windows LAPS
- Automated employee onboarding
- Automated employee offboarding
- Active Directory auditing
- Help Desk PowerShell toolkit
- Group Policy compliance reporting

### Core Infrastructure

- DNS forward and reverse lookup zones
- DHCP installation and scope configuration
- DHCP authorization troubleshooting
- Department file shares
- Share and NTFS permissions
- Group Policy drive mapping
- Folder Redirection
- Print server deployment
- File-share permission auditing
- Backup and file restoration

### Enterprise Operations

- Honey-account security monitoring
- PowerShell alert logging
- Windows Admin Center administration
- Process investigation
- Event Viewer analysis
- CPU and memory review
- Service troubleshooting
- Performance monitoring

---

## Selected Troubleshooting Scenarios

The lab includes problems I encountered and investigated rather than only successful configurations.

Examples include:

| Scenario | Investigation |
|---|---|
| IP connectivity worked but hostnames failed | Client DNS configuration, `nslookup`, DNS records, and resolver cache |
| DHCP stopped servicing clients | DHCP Event ID 1046 and Active Directory authorization |
| Group Policy did not apply | OU placement, GPO link, filtering, `gpupdate`, and `gpresult` |
| User received Access Denied | Security-group membership, share permissions, and NTFS permissions |
| Mapped drive did not appear | GPO scope and item-level targeting |
| Folder Redirection remained local | User policy scope, UNC access, permissions, and sign-in processing |
| Printer did not deploy | GPO processing, permissions, drivers, and Print Spooler status |
| Server appeared to use high CPU | Processes, System Idle Process, and sustained resource usage |
| Unexpected server shutdown events | Kernel-Power Event ID 41 and surrounding events |
| Honey-account activity detected | Security log review and PowerShell alert generation |

My troubleshooting process follows this model:

```text
See
  ↓
Think
  ↓
Examine
  ↓
Proceed
```

The goal is to collect evidence before making changes.

---

## Repository Roadmap

### 00 — Lab Setup

| Module | Status |
|---|:---:|
| Enterprise Virtualization | ✅ |
| Windows Server Installation | ✅ |
| Windows 11 Deployment | ✅ |

### 01 — Identity and Access Management

| Module | Status |
|---|:---:|
| Active Directory Domain Services | ✅ |
| Active Directory Administration | ✅ |
| Windows 11 Domain Join | ✅ |
| Group Policy Hardening | ✅ |
| Windows LAPS | ✅ |
| User Lifecycle Automation | ✅ |
| Offboarding Automation | ✅ |
| Active Directory Auditing | ✅ |
| Help Desk Automation | ✅ |
| Group Policy Compliance Reporting | ✅ |

### 02 — Core Infrastructure

| Module | Status |
|---|:---:|
| DNS Infrastructure | ✅ |
| DHCP Infrastructure | ✅ |
| File Services | ✅ |
| Folder Redirection | ✅ |
| Print Server Management | ✅ |
| File Server Auditing | ✅ |
| Backup and Disaster Recovery | ✅ |

### 03 — Enterprise Operations

| Module | Status |
|---|:---:|
| Security Monitoring with Honey Accounts | ✅ |
| Windows Admin Center | 🟨 |
| WSUS Patch Management | ⬜ |
| Server Monitoring | ⬜ |
| Remote Administration | ⬜ |
| Documentation and Knowledge Base | ⬜ |

### 04 — Cloud Identity and Microsoft 365

| Module | Status |
|---|:---:|
| Microsoft Entra ID | ⬜ |
| Hybrid Identity | ⬜ |
| Microsoft 365 Administration | ⬜ |
| MFA and Conditional Access | ⬜ |
| Identity Governance | ⬜ |

### 05 — Security Operations

| Module | Status |
|---|:---:|
| Sysmon Deployment | ⬜ |
| Microsoft Defender | ⬜ |
| Microsoft Sentinel | ⬜ |
| Threat Hunting | ⬜ |
| Incident Response | ⬜ |

### 06 — Governance, Risk, and Compliance

| Module | Status |
|---|:---:|
| NIST Cybersecurity Framework | ⬜ |
| CIS Benchmarks | ⬜ |
| Risk Assessment | ⬜ |
| Control Mapping | ⬜ |
| Audit and Compliance | ⬜ |

```text
✅ Completed
🟨 In progress
⬜ Planned
```

---

## Technical Skills

### Systems Administration

- Windows Server 2025
- Windows 11 Enterprise
- Server Manager
- Windows Admin Center
- Windows services
- Event Viewer
- Performance monitoring
- Backup and recovery

### Identity and Access Management

- Active Directory Domain Services
- Organizational Unit design
- User and group administration
- Role-based access concepts
- Joiner, Mover, and Leaver workflows
- Windows LAPS
- Delegated administration
- Account auditing

### Core Infrastructure

- DNS
- DHCP
- SMB file sharing
- Share and NTFS permissions
- Folder Redirection
- Group Policy drive mapping
- Print server administration
- Group Policy deployment

### Automation and Reporting

- PowerShell
- Active Directory PowerShell module
- CSV-based automation
- User onboarding scripts
- Offboarding scripts
- Permission reporting
- Group Policy reporting
- Event-log monitoring

### Troubleshooting

- Name-resolution problems
- IP configuration
- DHCP authorization
- Domain connectivity
- Group Policy processing
- File-access failures
- Service failures
- Event-log investigation
- CPU and memory investigation

### Documentation

- Technical README files
- Runbooks
- Troubleshooting procedures
- Validation checklists
- Architecture documentation
- Incident notes
- Screenshots and evidence collection

---

## Technologies

<p align="left">

<img src="https://img.shields.io/badge/Windows%20Server-0078D4?style=for-the-badge&logo=windows&logoColor=white" alt="Windows Server">

<img src="https://img.shields.io/badge/Windows%2011-0078D4?style=for-the-badge&logo=windows11&logoColor=white" alt="Windows 11">

<img src="https://img.shields.io/badge/Active%20Directory-0078D4?style=for-the-badge&logo=microsoft&logoColor=white" alt="Active Directory">

<img src="https://img.shields.io/badge/Group%20Policy-5E5E5E?style=for-the-badge&logo=microsoft&logoColor=white" alt="Group Policy">

<img src="https://img.shields.io/badge/PowerShell-5391FE?style=for-the-badge&logo=powershell&logoColor=white" alt="PowerShell">

<img src="https://img.shields.io/badge/Windows%20Admin%20Center-0078D4?style=for-the-badge&logo=microsoft&logoColor=white" alt="Windows Admin Center">

<img src="https://img.shields.io/badge/Microsoft%20Entra%20ID-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white" alt="Microsoft Entra ID">

<img src="https://img.shields.io/badge/Microsoft%20365-D83B01?style=for-the-badge&logo=microsoftoffice&logoColor=white" alt="Microsoft 365">

<img src="https://img.shields.io/badge/VMware%20Workstation-607078?style=for-the-badge&logo=vmware&logoColor=white" alt="VMware Workstation">

<img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub">

<img src="https://img.shields.io/badge/Git- F05032?style=for-the-badge&logo=git&logoColor=white" alt="Git">

</p>

---

## How I Document My Work

I organize each project around the complete operational lifecycle:

```text
Business Requirement
        ↓
Technology and Architecture
        ↓
Implementation
        ↓
Validation
        ↓
Troubleshooting
        ↓
Security Review
        ↓
Automation
        ↓
Lessons Learned
```

I include commands and screenshots, but I also document why a configuration exists, how I verified it, what could fail, and how I would troubleshoot it.

The purpose of the repository is to show how I approach technical problems, not only which products I have installed.

---

## Current Focus

I am currently working on:

- Windows Admin Center performance monitoring
- Server health investigation
- WSUS and patch-management planning
- PowerShell script improvement
- Microsoft Entra ID
- Hybrid identity
- Microsoft 365 administration
- Windows security monitoring
- Incident-response fundamentals

---

## Certifications and Learning

- Google IT Support Professional Certificate
- ISC2 Certified in Cybersecurity — In progress
- Microsoft Learn — Windows Server, Entra ID, and Microsoft 365
- TryHackMe — Windows, Active Directory, and Blue Team learning paths

---

## Career Direction

I am preparing for entry-level and junior roles such as:

- IT Support Specialist
- Help Desk Technician
- Service Desk Analyst
- Junior Systems Administrator
- Infrastructure Support Engineer
- Identity and Access Management Analyst
- Microsoft 365 Administrator
- Junior SOC Analyst

I am particularly interested in roles that combine user support, infrastructure administration, identity management, troubleshooting, and automation.

---

## Contact

<a href="https://www.linkedin.com/in/derrickperez2002/">
  <img src="https://img.shields.io/badge/LinkedIn-Derrick%20Perez-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
</a>

<a href="mailto:derickernestp@gmail.com">
  <img src="https://img.shields.io/badge/Email-derickernestp%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email">
</a>

---

<div align="center">

### Building practical experience through infrastructure deployment, troubleshooting, automation, and documentation.

[View the IT Operations Homelab](https://github.com/derrickernestperez/IT-Operations-Homelab)

</div>
