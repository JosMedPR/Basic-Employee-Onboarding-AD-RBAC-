# Basic-Employee-Onboarding-AD-RBAC-
Active Directory infrastructure rebuild for a fictional company called “Northstar Medical Group”. Includes domain setup, organizational structure, user provisioning, RBAC implementation, and incident resolution.

## Problem Statement
Northstar Medical Group ran into serious operational and security issues after outsourcing its identity management to an MSP. The result was a messy, undocumented Active Directory: accounts were set up manually without standard rules, people ended up with permissions they shouldn't have had, and former staff still had access months after leaving. Onboarding ground to a halt because organizational structure was practically nonexistent. In a healthcare setting, this lack of control and audit tracking wasn't just an IT headache; it put the organization at serious risk of major HIPAA violations and crippling fines.

## Solution Overview
To fix these security and compliance gaps, we rebuilt the environment from scratch with a standardized Active Directory domain (NMG.com). We structured dedicated Organizational Units (OUs) for HR, Finance, IT, and Operations, pairing them with security groups to enforce true Role-Based Access Control (RBAC). Instead of manual setup, automated assignments now ensure staff only receive the drives and resources required for their roles. Every account is provisioned under a strict principle of least privilege with full user metadata, cutting human error and locking down access. To verify everything worked in practice, we tested the new workflows against real-world support tickets, such as onboarding issue NMG-0047, to ensure day-one readiness for new hires.

## Video Walkthrough
[Walkthrough Video Coming Soon - Link will be added after recording]

## Tools Used
* Windows Server
* Active Directory Domain Services
* VirtualBox
* UTM
* RBAC
* GitHub

## Project Timeline
* Day 1: Domain creation and domain controller promotion
* Day 2: Organizational unit and security group design
* Day 3: User provisioning and RBAC implementation
* Day 4: Incident response and resolution (NMG-0047)
* Day 5: Documentation and case study packaging

## Key Accomplishments
* Built NMG.com domain from scratch
* Designed department-based OU structure (Finance, HR, IT, Operations)
* Implemented RBAC with security groups mapped to each department
* Provisioned 15 user accounts with consistent naming conventions and attribute standards
* Diagnosed and resolved a multi-cause access issue (wrong OU + missing group membership)
* Documented full incident resolution with root cause analysis

## Repository Structure

Basic-Employee-Onboarding-AD-RBAC/
├── Documentation/
│   ├── Domain Config File.txt
│   ├── Security Group Doc.txt
│   ├── User List Documentation.txt
│   └── RBAC-Structure.md
├── Incident-Reports/
│   └── NMG-0047-Resolution.txt
├── Screenshots/
│   ├── Day1-AD-Users-and-Computers-showing.png
│   ├── Day1-Dcdiag-Results.png
│   ├── Day1-Server-Manager.png
│   ├── Day2-All-four-OUs.png
│   ├── Day2-Security-Group-Finance.png
│   ├── Day2-Security-Group-HR.png
│   ├── Day2-Security-Group-IT.png
│   ├── Day2-Security-Group-Operations.png
│   ├── Day3-Final-expanded-tree.png
│   ├── Day3-Group-membership-of-Finance-OU.png
│   ├── Day3-Group-membership-of-HR-OU.png
│   ├── Day3-Group-membership-of-IT-OU.png
│   ├── Day3-Group-membership-of-Operations-OU.png
│   ├── Day3-Users-inside-Finance-OU.png
│   ├── Day3-Users-inside-HR-OU.png
│   ├── Day3-Users-inside-IT-OU.png
│   ├── Day3-Users-inside-Operations-OU.png
│   ├── Day4-Jane's-corrected-OU.png
│   ├── Day4-Jane's-corrected-group-membership.png
│   └── Day4-Jane's-incorrect-OU-placement.png
└── README.md

* /Documentation:Contains infrastructure baseline configurations, security group design specifications, directory user rosters, and access mapping documentation.

   * Domain Config File: Baseline domain parameters, DC hostname, static IP configuration, and creation date.
   
   * Security Group Doc: Breakdown of OU names, corresponding security groups, and operational purposes.
   
   * RBAC-Structure.md: Full RBAC matrix mapping departmental OUs, security groups, assigned members, and system access scopes.
   
   * User List Documentation: Complete roster of 15 provisioned users, their UPNs, departments, titles, and group assignments.

* /Incident-Reports:* Contains documentation and root-cause analysis for administrative support escalations.
   
   * NMG-0047-Resolution.txt: Detailed post-incident write-up documenting the investigation, misconfiguration discovery, remediation steps, and resolution confirmation for Jane Cooper's account.

* /Screenshots: Visual validation covering every stage of deployment, directory hierarchy, user provisioning, and incident resolution:

   * Day 1 (Domain Setup): Verification in Active Directory Users and Computers (ADUC), successful dcdiag domain health check output, and Server Manager status.
   
   * Day 2 (OU & Security Group Architecture): View of all four departmental OUs, plus individual evidence captures for the Finance, HR, IT, and Operations security groups.
   
   * Day 3 (User Provisioning & RBAC Validation): Department-by-department proof of users inside each OU, membership verification for each security group, and the final expanded AD tree hierarchy.
   
   * Day 4 (Incident NMG-0047 Remediation): Evidence captures showing Jane Cooper's initial incorrect OU placement, relocation to the HR OU, and assignment to the HR-Users security group.
