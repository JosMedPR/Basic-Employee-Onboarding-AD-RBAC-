# Basic-Employee-Onboarding-AD-RBAC-
Active Directory infrastructure rebuild for a fictional company called “Northstar Medical Group”. Includes domain setup, organizational structure, user provisioning, RBAC implementation, and incident resolution.

# Basic Employee Onboarding (AD)(RBAC)

## Problem Statement
Northstar Medical Group ran into serious operational and security issues after outsourcing its identity management to an MSP. The result was a messy, undocumented Active Directory: accounts were set up manually without standard rules, people ended up with permissions they shouldn't have had, and former staff still had access months after leaving. Onboarding ground to a halt because organizational structure was practically nonexistent. In a healthcare setting, this lack of control and audit tracking wasn't just an IT headache; it put the organization at serious risk of major HIPAA violations and crippling fines.

## Solution Overview
To fix these security and compliance gaps, we rebuilt the environment from scratch with a standardized Active Directory domain (NMG.com). We structured dedicated Organizational Units (OUs) for HR, Finance, IT, and Operations, pairing them with security groups to enforce true Role-Based Access Control (RBAC). Instead of manual setup, automated assignments now ensure staff only receive the drives and resources required for their roles. Every account is provisioned under a strict principle of least privilege with full user metadata, cutting human error and locking down access. To verify everything worked in practice, we tested the new workflows against real-world support tickets, such as onboarding issue NMG-0047, to ensure day-one readiness for new hires.

## Video Walkthrough
[Add your video walkthrough link placeholder here. You will record this tomorrow and update this link so visitors can see a live demonstration of your lab environment.]

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
* [Add your second key accomplishment here]
* [Add your third key accomplishment here]
