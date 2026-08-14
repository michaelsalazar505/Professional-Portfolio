Windows Infrastructure and Administration Portfolio

Enterprise-style Windows administration projects built and documented by Michael Salazar.

This portfolio follows one progressive lab environment rather than isolated demonstrations. Each project extends the same Windows enterprise environment, preserves earlier design decisions, and adds validated administrative capabilities.

Environment Overview

Component

Implementation

Hypervisor

Microsoft Hyper-V on Windows 11 Pro

Domain controller

CORP-DC1 - Windows Server 2025

Member server

CORP-SRV01 - Windows Server 2025

Management workstation

MGMT-CL01 - Windows 11 Pro

Active Directory forest

corp.mslab.test

Corporate network

172.16.10.0/24

Core administration tools

Hyper-V Manager, Server Manager, ADUC, DNS Manager, and PowerShell

Portfolio Progress

Status

Count

Completed and documented projects

5

Current portfolio release

Project 05

Planned progressive lab sequence

14 projects

Completed Projects

1. Hyper-V Enterprise Lab Foundation

Built the virtualization foundation for a multi-system Windows enterprise lab.

Enabled and validated Hyper-V on Windows 11 Pro.

Created standardized folders for virtual machines, VHDX files, ISOs, exports, and evidence.

Designed isolated corporate and branch virtual switches.

Deployed Windows Server 2025 on CORP-DC1 and CORP-SRV01.

Deployed Windows 11 Pro on MGMT-CL01.

Established checkpoints and repeatable VM configuration practices.

View Project 01 PDF

2. Active Directory Forest Deployment

Deployed the identity and name-resolution foundation for the enterprise environment.

Assigned a static IPv4 configuration to CORP-DC1.

Installed Active Directory Domain Services and DNS.

Promoted CORP-DC1 as the first domain controller.

Created the corp.mslab.test forest and domain.

Validated AD DS, DNS, forest health, and domain-controller discovery.

Preserved a pre-deployment rollback checkpoint.

View Project 02 PDF

3. Active Directory Organizational Unit Design

Created a scalable OU hierarchy for administration, policy targeting, and lifecycle management.

Created the protected Corp parent OU.

Separated users by Finance, Human Resources, Information Technology, and Operations.

Created server, desktop, laptop, administrative-account, service-account, stale-account, and stale-computer OUs.

Added a corporate desktop hierarchy for management workstations.

Enabled protection against accidental deletion.

Validated OU creation and protection with PowerShell.

View Project 03 PDF

4. Active Directory User and Group Administration

Implemented departmental identities, role-based access foundations, privileged-account separation, and offboarding controls.

Provisioned and classified eight departmental users.

Created Global and Domain Local security groups.

Implemented the AGDLP path: Accounts to Global groups to Domain Local groups to future Permissions.

Created the separate adm_msalazar privileged identity.

Protected the administrative identity from delegation.

Created a disabled and unprivileged svc_labbackup placeholder.

Offboarded mreed by removing access, disabling the identity, documenting the action, and moving it to Stale Accounts.

Validated account states, group membership, nesting, and OU placement with PowerShell.

View Project 04 PDF

5. Domain Join and Computer Account Management

Integrated the server and management workstation into Active Directory and validated their machine trusts.

Diagnosed APIPA addressing caused by the private Hyper-V network having no DHCP service.

Configured CORP-SRV01 as 172.16.10.20/24 and MGMT-CL01 as 172.16.10.30/24.

Configured CORP-DC1 at 172.16.10.10 as the exclusive AD DNS server.

Validated domain, host, and LDAP SRV record resolution before joining.

Joined CORP-SRV01 and MGMT-CL01 to corp.mslab.test.

Confirmed PartOfDomain = True and healthy secure channels on both systems.

Validated domain authentication as CORP\msalazar on MGMT-CL01.

Confirmed enabled computer objects and deliberate placement in the Servers and Corporate Desktops OUs.

View Project 05 PDF

Skills Demonstrated

Hyper-V deployment and virtual-network design

Windows Server 2025 installation and administration

Active Directory Domain Services and integrated DNS

Forest, domain, OU, user, group, and computer administration

AGDLP authorization design

Privileged-account separation and least privilege

Identity provisioning and offboarding

Static IPv4 configuration and AD DNS troubleshooting

Domain joins, authentication, and secure-channel validation

PowerShell-based configuration verification

Change control, checkpoints, evidence capture, and technical documentation

Planned Lab Progression

The environment will continue to expand through file services and NTFS/share permissions, Group Policy, DHCP, remote administration, event collection and monitoring, branch services, security hardening, backup and recovery, automation, and final enterprise validation.

Repository

Return to the Professional Portfolio

Contact

Michael Salazar
Santa Fe, New Mexico
Michaelsalazar505@gmail.com
GitHub Portfolio
