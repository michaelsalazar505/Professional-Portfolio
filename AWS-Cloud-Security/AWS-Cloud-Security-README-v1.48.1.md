# AWS Cloud Security Engineering Portfolio

**Portfolio Version:** `v1.48.1`
**Projects Completed:** `49`
**Owner:** Michael Salazar
**Status:** Active / In Progress

---

## Portfolio Summary

This repository documents a hands-on AWS cloud security lab portfolio. The work progresses from account hardening and identity foundations into AWS Organizations, logging, delegated administration, threat detection, alerting, advanced IAM guardrails, cloud networking, Infrastructure as Code, workload-level network security, private compute administration, private AWS service access, SSH replacement with AWS Systems Manager Session Manager, auditable Session Manager logging, exposure-driven GuardDuty detection, static credential risk, EC2 Instance Metadata Service credential exposure, EC2 user data secret exposure, GuardDuty cryptomining detection, EBS snapshot-based cloud forensics, and S3 public access misconfiguration analysis.

The first forty-nine projects form a connected security foundation, now moving from static organization guardrails into multi-region, event-driven security automation and autoremediation architecture.

---

## Architecture Progression

```text
Project 01 - Secure AWS Management Account
        |
        v
Project 02 - Secure IAM Administrator Account
        |
        v
Project 03 - CloudTrail Management Event Logging
        |
        v
Project 04 - CloudFormation SecurityAlerts Topic
        |
        v
Project 05 - Billing Alerts and SNS Email
        |
        v
Project 06 - EC2 IAM Role for Systems Manager
        |
        v
Project 07 - CloudTrail S3 ReadWrite IAM Policy
        |
        v
Project 08 - AWS Organizations Security OU and SecurityAudit Account
        |
        v
Project 09 - Service Control Policy Guardrails
        |
        v
Project 10 - Cross-Account Role Assumption and Logging Bucket
        |
        v
Project 11 - Centralized Logging Bucket Policy
        |
        v
Project 12 - Organization CloudTrail to SecurityAudit Bucket
        |
        v
Project 13 - IAM Identity Center SSO and MFA Foundation
        |
        v
Project 14 - AdministratorAccess Permission Set Assignment
        |
        v
Project 15 - Enterprise AWS Organizations OU Structure
        |
        v
Project 16 - SCP Target Rework and LogArchive Recovery
        |
        v
Project 17 - RegionLockout SCP
        |
        v
Project 18 - S3 Lifecycle Cost Control for CloudTrail Logs
        |
        v
Project 19 - Button Up Organization Contacts and Workload OUs
        |
        v
Project 20 - Delegated Administration for IAM Identity Center and CloudTrail
        |
        v
Project 21 - Security Team Permission Sets in IAM Identity Center
        |
        v
Project 22 - Multi-Region GuardDuty Delegated Administration
        |
        v
Project 23 - Security Hub Central Configuration
        |
        v
Project 24 - EventBridge Security Hub Alerts to SNS Email
        |
        v
Project 25 - IAM Identity Center Manage Policies Permission Set
        |
        v
Project 26 - IAM Identity Center Permissions Boundary
        |
        v
Project 27 - Default VPC Exploration and Cleanup
        |
        v
Project 28 - Custom VPC Public Subnets and Internet Gateway Routing
        |
        v
Project 29 - Private Subnets and NAT Gateway Egress
        |
        v
Project 30 - CloudFormation VPC Infrastructure as Code
        |
        v
Project 31 - VPC Security Groups and Security Group References
        |
        v
Project 32 - Private EC2 Instance with Session Manager
        |
        v
Project 33 - Private Subnet Access with VPC Endpoints
        |
        v
Project 34 - Session Manager Run As and CLI Access
        |
        v
Project 35 - Session Manager S3 Logging
        |
        v
Project 36 - GuardDuty Public SSH Exposure
        |
        v
Project 37 - Access Key Exposure and Static Credentials
        |
        v
Project 38 - IMDSv1 and IMDSv2 Metadata Credential Risk
        |
        v
Project 39 - EC2 User Data Secret Exposure
        |
        v
Project 40 - User Data Cryptomining GuardDuty Detection
        |
        v
Project 41 - EBS Forensic Snapshot and Cross-Account Sharing
        |
        v
Project 42 - Forensics Volume Snapshot Analysis
        |
        v
Project 43 - S3 ACL Public Bucket Exposure
        |
        v
Project 44 - S3 Misconfigured Bucket Policy Exposure
        |
        v
Project 45 - S3 Resource Control Policy Prod Guardrail
        |
        v
Project 46 - IAM Access Analyzer Delegated External Access
        |
        v
Project 47 - S3 Block Public Access Bucket and Account Controls
        |
        v
Project 48 - EC2 Declarative Policy IMDSv2 Enforcement
        |
        v
Project 49 - EventBridge Security Automation and Broken RCP Replacement
```

---

## Completed Projects

| # | Project | Version | Status | Focus |
|---|---------|---------|--------|-------|
| 01 | Secure AWS Management Account | `v1.0.1` | Complete | Root account hardening, MFA, no root access keys |
| 02 | Secure IAM Administrator Account | `v1.0.1` | Complete | IAM admin user, Administrators group, MFA, no access keys |
| 03 | CloudTrail Management Event Logging | `v1.0.1` | Complete | Multi-region CloudTrail management event logging |
| 04 | CloudFormation SecurityAlerts Topic | `v1.0.1` | Complete | SNS topic deployment with CloudFormation |
| 05 | Billing Alerts and SNS Email | `v1.0.0` | Complete | Tiered billing alerts and email notification |
| 06 | EC2 IAM Role for Systems Manager | `v1.0.0` | Complete | EC2 trust policy and SSM managed instance role |
| 07 | CloudTrail S3 ReadWrite IAM Policy | `v1.0.0` | Complete | Customer-managed policy for CloudTrail S3 object access |
| 08 | AWS Organizations Security OU and SecurityAudit Account | `v1.0.0` | Complete | Organization, Security OU, and SecurityAudit member account |
| 09 | Service Control Policy Guardrails | `v1.0.0` | Complete | Root restriction and organization-leave prevention SCP |
| 10 | Cross-Account Role Assumption and Logging Bucket | `v1.0.0` | Complete | OrganizationAccountAccessRole and centralized S3 bucket creation |
| 11 | Centralized Logging Bucket Policy | `v1.0.0` | Complete | Restricted CloudTrail bucket/resource policy |
| 12 | Organization CloudTrail to SecurityAudit Bucket | `v1.0.0` | Complete | Organization trail redirected to centralized logging storage |
| 13 | IAM Identity Center SSO and MFA Foundation | `v1.0.0` | Complete | IAM Identity Center, MFA, admin group, SSO user |
| 14 | AdministratorAccess Permission Set Assignment | `v1.0.0` | Complete | AdministratorAccess permission set and SSO admin access validation |
| 15 | Enterprise AWS Organizations OU Structure | `v1.0.0` | Complete | Infrastructure, Workloads, Exceptions, Sandbox, Onboarding, Nursery, Suspended, IncidentResponse OUs |
| 16 | SCP Target Rework and LogArchive Recovery | `v1.0.0` | Complete | OU guardrail repair, root recovery, LogArchive rename, SecurityAudit recreation |
| 17 | RegionLockout SCP | `v1.0.0` | Complete | Region restriction to approved regions and global-service exceptions |
| 18 | S3 Lifecycle Cost Control for CloudTrail Logs | `v1.0.0` | Complete | 90-day lifecycle expiration for lab cost control |
| 19 | Button Up Organization Contacts and Workload OUs | `v1.0.0` | Complete | Trusted access, alternate contacts, Prod/Non-Prod OUs, TestAccount1 |
| 20 | Delegated Administration for IAM Identity Center and CloudTrail | `v1.0.0` | Complete | IAM delegated admin for Identity Center and SecurityAudit delegated admin for CloudTrail |
| 21 | Security Team Permission Sets in IAM Identity Center | `v1.0.0` | Complete | Security Administrators, IAM Administrators, ReadOnlyAccess, IdentityCenterAdmin, SecurityFullAdmin |
| 22 | Multi-Region GuardDuty Delegated Administration | `v1.0.0` | Complete | GuardDuty in us-west-2 and us-east-1 with SecurityAudit delegated admin |
| 23 | Security Hub Central Configuration | `v1.0.0` | Complete | Security Hub delegated admin, central configuration, standards disabled |
| 24 | EventBridge Security Hub Alerts to SNS Email | `v1.0.0` | Complete | SecurityHubFindings rule to SecurityHubAlerts SNS email |
| 25 | IAM Identity Center Manage Policies Permission Set | `v1.0.0` | Complete | Policy-management permissions for Identity Center administrators |
| 26 | IAM Identity Center Permissions Boundary | `v1.0.0` | Complete | SSOPermissionBoundary and self-escalation control |
| 27 | Default VPC Exploration and Cleanup | `v1.0.0` | Complete | Default VPC, subnets, route table, Internet Gateway, deletion after testing |
| 28 | Custom VPC Public Subnets and Internet Gateway Routing | `v1.0.0` | Complete | CloudSLAW VPC, public subnets, Internet Gateway, default route |
| 29 | Private Subnets and NAT Gateway Egress | `v1.0.0` | Complete | Private subnets, NAT Gateway, private route table, outbound-only Internet access, cleanup |
| 30 | CloudFormation VPC Infrastructure as Code | `v1.0.0` | Complete | YAML template, full VPC stack, dependency flowchart, stack validation, stack deletion |
| 31 | VPC Security Groups and Security Group References | `v1.0.0` | Complete | Database and Backup security groups, CIDR rules, NFS security-group reference, cleanup |
| 32 | Private EC2 Instance with Session Manager | `v1.0.0` | Complete | Amazon Linux EC2, private subnet, SSMClient instance profile, Session Manager access, cleanup |
| 33 | Private Subnet Access with VPC Endpoints | `v1.0.0` | Complete | Interface endpoints for ssm, ssmmessages, and ec2messages, private Session Manager access, cleanup |
| 34 | Session Manager Run As and CLI Access | `v1.0.0` | Complete | Run As ec2-user, SLAW/SLAW2 instances, AWS CLI start-session, SSH replacement pattern |
| 35 | Session Manager S3 Logging | `v1.0.0` | Complete | S3 session logging, SSMLogs inline policy, downloaded command log validation, cleanup |
| 36 | GuardDuty Public SSH Exposure | `v1.0.3` | Complete | Public SSH exposure, GuardDuty finding validation, redacted alert evidence, stack cleanup |
| 37 | Access Key Exposure and Static Credentials | `v1.0.0` | Complete | AKIA stack, IAM access key creation/deletion, exposed credentials in .aws profile, cleanup |
| 38 | IMDSv1 and IMDSv2 Metadata Credential Risk | `v1.0.0` | Complete | IMDS stack, IMDSv1 credential retrieval, IMDSv2 token requirement, SSRF risk analysis, cleanup |
| 39 | EC2 User Data Secret Exposure | `v1.0.0` | Complete | SLAW stack, dummy secrets in user data, IMDSv2 retrieval, CloudTrail sensitiveDataRemoved evidence, cleanup |
| 40 | User Data Cryptomining GuardDuty Detection | `v1.0.0` | Complete | cloud-init callback to defunct mining domain, GuardDuty HIGH finding validation, cleanup |
| 41 | EBS Forensic Snapshot and Cross-Account Sharing | `v1.0.0` | Complete | CSI stack, Hacked volume snapshot, CSI-Incident-1, shared with SecurityAudit |
| 42 | Forensics Volume Snapshot Analysis | `v1.0.0` | Complete | SecurityAudit Forensics stack, create CSI volume from shared snapshot, attach and mount volume, recover embedded evidence |
| 43 | S3 ACL Public Bucket Exposure | `v1.0.0` | Complete | Block Public Access disabled, ACLs enabled, Everyone List and Read permissions, Access Analyzer follow-up target |
| 44 | S3 Misconfigured Bucket Policy Exposure | `v1.0.0` | Complete | Public ListBucket/GetObject through wildcard principal and 0.0.0.0/0 bucket-policy statements |
| 45 | S3 Resource Control Policy Prod Guardrail | `v1.0.0` | Superseded - Removed in Project 49 | Enabled RCPs, created S3 Classified Sensitive, attached to Prod OU, intentionally broken deny behavior |
| 46 | IAM Access Analyzer Delegated External Access | `v1.0.0` | Complete - Findings Review Pending | SecurityAudit delegated admin, organization external analyzers, 17 active resources, email notification |
| 47 | S3 Block Public Access Bucket and Account Controls | `v1.0.0` | Complete - Analyzer Validation Pending | Broad BPA on BP bucket, new-only BPA on SLAW bucket, account-level BPA in SecurityAudit |
| 48 | EC2 Declarative Policy IMDSv2 Enforcement | `v1.0.0` | Complete | S3 status-report workflow, EC2 policy enablement, uniform report, IMDSv2 defaults attached to Prod |
| 49 | EventBridge Security Automation and Broken RCP Replacement | `v1.0.0` | Complete - Automation Buildout Pending | Removed defective S3 RCP and created SecurityAutomation custom event buses in us-east-1 and us-west-2 |
---

## Latest Project - Project 49: EventBridge Security Automation and Broken RCP Replacement

Detached and deleted the defective `S3 Classified Sensitive` RCP, then moved into the `SecurityOperations` account and created `SecurityAutomation` custom Amazon EventBridge buses in `us-east-1` and `us-west-2`. Each bus uses an organization-scoped resource policy permitting `events:PutEvents` only when `aws:PrincipalOrgID` matches the AWS Organization.

### Implemented

- S3 Classified Sensitive RCP detachment
- S3 Classified Sensitive RCP deletion
- SecurityOperations automation account
- Custom EventBridge `SecurityAutomation` event bus
- `us-east-1` event bus
- `us-west-2` event bus
- Cross-account `events:PutEvents`
- `aws:PrincipalOrgID` organization restriction
- Regional resource ARN handling
- Central event-ingestion foundation
- Future autoremediation architecture

### Why It Matters

The previous RCP could not enforce the desired sensitive-bucket tag invariant. Instead of replacing it with an overly broad deny, the portfolio now uses an event-driven automation pattern. The two custom event buses will receive selected security and CloudTrail events from organization accounts and drive targeted remediation in future labs.

## AWS Services and Technologies Used

| Area | Services and Technologies |
|------|---------------------------|
| Identity | AWS IAM, MFA, IAM Roles, AWS STS, IAM Identity Center, Instance Profiles |
| Compute | Amazon EC2, Amazon Linux, EC2 User Data, EC2 Instance Metadata Service, EC2 Instance Metadata Defaults |
| Systems Management | AWS Systems Manager Session Manager, AWS CLI Session Manager access |
| Logging | AWS CloudTrail, Session Manager S3 logging |
| Storage | Amazon S3, S3 ACLs, S3 Bucket Policies, S3 Block Public Access, S3 Object Ownership, Amazon EBS, EBS Volumes, EBS Snapshots |
| Infrastructure as Code | AWS CloudFormation, YAML |
| Notifications | Amazon SNS |
| Monitoring | Amazon CloudWatch |
| Financial Monitoring | AWS Billing and Cost Management |
| Governance | AWS Organizations, Service Control Policies, Resource Control Policies, EC2 Declarative Policies, AWS Account Management |
| Threat Detection | Amazon GuardDuty, AWS Security Hub, IAM Access Analyzer |
| Eventing | Amazon EventBridge |
| Networking | Amazon VPC, VPC Endpoints, AWS PrivateLink, Security Groups, NAT Gateway, Internet Gateway, Route Tables, Elastic IP, Network ACLs, DHCP Options |
| Cloud Forensics | Cross-account snapshot sharing, volume mounting, Linux file-system analysis |
| Secrets Management | AWS Secrets Manager and SSM Parameter Store recommended as production alternatives |

---

## Regions Used

| Region | Name | Portfolio Usage |
|--------|------|-----------------|
| `us-west-2` | US West (Oregon) | Primary lab region, CloudTrail, CloudFormation, SNS, GuardDuty, Security Hub, EventBridge, VPC, Security Groups, NAT Gateway, EC2, VPC Endpoints, Session Manager, S3 session logs, IMDS testing, user data testing, EBS snapshots, forensic volumes, S3 ACL testing |
| `us-east-1` | US East (N. Virginia) | Billing alarms, CloudFormation, SNS, GuardDuty |
| `us-east-2` | US East (Ohio) | CloudTrail |

---

## Documentation Standard

Each project PDF follows the same portfolio format: cover page, executive summary, business problem, objectives, environment, architecture/workflow diagram, implementation summary, evidence, security analysis, lessons learned, production improvements, skills, resume bullet, STAR story, version history, and references.

Every provided screenshot is embedded as project evidence, numbered, captioned, and explained. Sensitive account identifiers, resource identifiers, access keys, secret access keys, session tokens, and real credentials are redacted where visible.

---

## Repository Structure

```text
AWS-Cloud-Security/
|
|-- README.md
|
|-- 01-Secure-AWS-Management-Account/
|   |-- README.md
|   |-- Project_01_*.pdf
|   `-- screenshots/
|-- 02-Secure-IAM-Administrator-Account/
|   |-- README.md
|   |-- Project_02_*.pdf
|   `-- screenshots/
|-- 03-CloudTrail-Management-Event-Logging/
|   |-- README.md
|   |-- Project_03_*.pdf
|   `-- screenshots/
|-- 04-CloudFormation-SecurityAlerts-Topic/
|   |-- README.md
|   |-- Project_04_*.pdf
|   `-- screenshots/
|-- 05-Billing-Alerts-and-SNS-Email/
|   |-- README.md
|   |-- Project_05_*.pdf
|   `-- screenshots/
|-- 06-EC2-IAM-Role-for-Systems-Manager/
|   |-- README.md
|   |-- Project_06_*.pdf
|   `-- screenshots/
|-- 07-CloudTrail-S3-ReadWrite-IAM-Policy/
|   |-- README.md
|   |-- Project_07_*.pdf
|   `-- screenshots/
|-- 08-AWS-Organizations-Security-OU-and-SecurityAudit-Account/
|   |-- README.md
|   |-- Project_08_*.pdf
|   `-- screenshots/
|-- 09-Service-Control-Policy-Guardrails/
|   |-- README.md
|   |-- Project_09_*.pdf
|   `-- screenshots/
|-- 10-Cross-Account-Role-Assumption-and-Logging-Bucket/
|   |-- README.md
|   |-- Project_10_*.pdf
|   `-- screenshots/
|-- 11-Centralized-Logging-Bucket-Policy/
|   |-- README.md
|   |-- Project_11_*.pdf
|   `-- screenshots/
|-- 12-Organization-CloudTrail-to-SecurityAudit-Bucket/
|   |-- README.md
|   |-- Project_12_*.pdf
|   `-- screenshots/
|-- 13-IAM-Identity-Center-SSO-and-MFA-Foundation/
|   |-- README.md
|   |-- Project_13_*.pdf
|   `-- screenshots/
|-- 14-AdministratorAccess-Permission-Set-Assignment/
|   |-- README.md
|   |-- Project_14_*.pdf
|   `-- screenshots/
|-- 15-Enterprise-AWS-Organizations-OU-Structure/
|   |-- README.md
|   |-- Project_15_*.pdf
|   `-- screenshots/
|-- 16-SCP-Target-Rework-and-LogArchive-Recovery/
|   |-- README.md
|   |-- Project_16_*.pdf
|   `-- screenshots/
|-- 17-RegionLockout-SCP/
|   |-- README.md
|   |-- Project_17_*.pdf
|   `-- screenshots/
|-- 18-S3-Lifecycle-Cost-Control-for-CloudTrail-Logs/
|   |-- README.md
|   |-- Project_18_*.pdf
|   `-- screenshots/
|-- 19-Button-Up-Organization-Contacts-and-Workload-OUs/
|   |-- README.md
|   |-- Project_19_*.pdf
|   `-- screenshots/
|-- 20-Delegated-Administration-for-IAM-Identity-Center-and-CloudTrail/
|   |-- README.md
|   |-- Project_20_*.pdf
|   `-- screenshots/
|-- 21-Security-Team-Permission-Sets-in-IAM-Identity-Center/
|   |-- README.md
|   |-- Project_21_*.pdf
|   `-- screenshots/
|-- 22-Multi-Region-GuardDuty-Delegated-Administration/
|   |-- README.md
|   |-- Project_22_*.pdf
|   `-- screenshots/
|-- 23-Security-Hub-Central-Configuration/
|   |-- README.md
|   |-- Project_23_*.pdf
|   `-- screenshots/
|-- 24-EventBridge-Security-Hub-Alerts-to-SNS-Email/
|   |-- README.md
|   |-- Project_24_*.pdf
|   `-- screenshots/
|-- 25-IAM-Identity-Center-Manage-Policies-Permission-Set/
|   |-- README.md
|   |-- Project_25_*.pdf
|   `-- screenshots/
|-- 26-IAM-Identity-Center-Permissions-Boundary/
|   |-- README.md
|   |-- Project_26_*.pdf
|   `-- screenshots/
|-- 27-Default-VPC-Exploration-and-Cleanup/
|   |-- README.md
|   |-- Project_27_*.pdf
|   `-- screenshots/
|-- 28-Custom-VPC-Public-Subnets-and-Internet-Gateway-Routing/
|   |-- README.md
|   |-- Project_28_*.pdf
|   `-- screenshots/
|-- 29-Private-Subnets-and-NAT-Gateway-Egress/
|   |-- README.md
|   |-- Project_29_*.pdf
|   `-- screenshots/
|-- 30-CloudFormation-VPC-Infrastructure-as-Code/
|   |-- README.md
|   |-- Project_30_*.pdf
|   `-- screenshots/
|-- 31-VPC-Security-Groups-and-Security-Group-References/
|   |-- README.md
|   |-- Project_31_*.pdf
|   `-- screenshots/
|-- 32-Private-EC2-Instance-with-Session-Manager/
|   |-- README.md
|   |-- Project_32_*.pdf
|   `-- screenshots/
|-- 33-Private-Subnet-Access-with-VPC-Endpoints/
|   |-- README.md
|   |-- Project_33_*.pdf
|   `-- screenshots/
|-- 34-Session-Manager-Run-As-and-CLI-Access/
|   |-- README.md
|   |-- Project_34_*.pdf
|   `-- screenshots/
|-- 35-Session-Manager-S3-Logging/
|   |-- README.md
|   |-- Project_35_*.pdf
|   `-- screenshots/
|-- 36-GuardDuty-Public-SSH-Exposure/
|   |-- README.md
|   |-- Project_36_*.pdf
|   `-- screenshots/
|-- 37-Access-Key-Exposure-and-Static-Credentials/
|   |-- README.md
|   |-- Project_37_*.pdf
|   `-- screenshots/
|-- 38-IMDSv1-and-IMDSv2-Metadata-Credential-Risk/
|   |-- README.md
|   |-- Project_38_*.pdf
|   `-- screenshots/
|-- 39-EC2-User-Data-Secret-Exposure/
|   |-- README.md
|   |-- Project_39_*.pdf
|   `-- screenshots/
|-- 40-User-Data-Cryptomining-GuardDuty-Detection/
|   |-- README.md
|   |-- Project_40_*.pdf
|   `-- screenshots/
|-- 41-EBS-Forensic-Snapshot-and-Cross-Account-Sharing/
|   |-- README.md
|   |-- Project_41_*.pdf
|   `-- screenshots/
|-- 42-Forensics-Volume-Snapshot-Analysis/
|   |-- README.md
|   |-- Project_42_*.pdf
|   `-- screenshots/
|-- 43-S3-ACL-Public-Bucket-Exposure/
|   |-- README.md
|   |-- Project_43_*.pdf
|   `-- screenshots/
|-- 44-S3-Misconfigured-Bucket-Policy-Exposure/
|   |-- README.md
|   |-- Project_44_*.pdf
|   `-- screenshots/
|-- 45-S3-Resource-Control-Policy-Prod-Guardrail/
|   |-- README.md
|   |-- Project_45_*.pdf
|   `-- screenshots/
|-- 46-IAM-Access-Analyzer-Delegated-External-Access/
|   |-- README.md
|   |-- Project_46_*.pdf
|   `-- screenshots/
|-- 47-S3-Block-Public-Access-Bucket-and-Account-Controls/
|   |-- README.md
|   |-- Project_47_*.pdf
|   `-- screenshots/
|-- 48-EC2-Declarative-Policy-IMDSv2-Enforcement/
|   |-- README.md
|   |-- Project_48_*.pdf
|   `-- screenshots/
|-- 49-EventBridge-Security-Automation-Broken-RCP-Replacement/
|   |-- README.md
|   |-- Project_49_*.pdf
|   `-- screenshots/
|
`-- Resources/
    |-- Documentation-Standard.pdf
    `-- Diagrams/
```

---

## Portfolio Metrics

| Metric | Current Value |
|--------|---------------|
| Portfolio Version | `v1.48.1` |
| Completed AWS Projects | `49` |
| AWS Services / Technologies Used | `25` |
| Embedded Project Screenshots | `132` |
| Architecture Diagrams | `47` |
| Project PDFs | `49` |

---

## Portfolio Version History

## `v1.48.1` - Raw-Friendly README Formatting

### Updated

- Converted repository trees to ASCII-only characters.
- Removed emoji and decorative Unicode status symbols.
- Replaced smart punctuation with plain ASCII equivalents.
- Removed trailing whitespace and normalized line endings.
- Preserved standard GitHub Markdown headings, tables, links, checklists, and fenced code blocks.
- Established raw-friendly Markdown as the README format for future portfolio updates.

---


## `v1.48.0` - EventBridge Security Automation and Broken RCP Replacement

### Added

- Project 49 documentation
- Broken `S3 Classified Sensitive` RCP removal
- SecurityOperations automation architecture
- `SecurityAutomation` custom EventBridge buses in us-east-1 and us-west-2
- Organization-scoped `events:PutEvents` resource policy
- `aws:PrincipalOrgID` policy analysis
- Future EventBridge, Lambda, and StackSets remediation roadmap

### Updated

- Project 45 status changed to `Superseded - Removed in Project 49`

---

## `v1.47.0` - EC2 Declarative Policy IMDSv2 Enforcement

### Added

- Project 48 documentation
- `us-east-1` declarative-policy report bucket
- Reporting-service S3 bucket policy
- EC2 policy type enablement
- Organization account status report
- Uniform settings and zero inconsistent accounts evidence
- IMDSv2 Instance Metadata Defaults policy
- Prod OU attachment evidence

---

## `v1.46.0` - S3 Block Public Access Bucket and Account Controls

### Added

- Project 47 documentation
- BP bucket broad ACL and policy blocking
- SLAW bucket new-only ACL and policy blocking
- SecurityAudit account-level Block all public access
- Immediate versus staged remediation comparison
- Access Analyzer verification follow-up

---

## `v1.45.0` - IAM Access Analyzer Delegated External Access

### Added

- Project 46 documentation
- SecurityAudit delegated-administrator configuration
- Oregon and N. Virginia external access analyzers
- Current-organization zone of trust
- Active finding evidence showing 17 resources
- Security Hub email-notification validation
- Data-perimeter detection and remediation planning

---

## `v1.44.0` - S3 Resource Control Policy Prod Guardrail

### Added

- Project 45 documentation
- Resource Control Policies enablement
- `S3 Classified Sensitive` customer-managed RCP
- Direct Prod OU attachment evidence
- Explicit-deny and data-perimeter analysis
- Intentionally broken policy behavior warning
- Future RCP remediation requirement

---

## `v1.43.0` - S3 Misconfigured Bucket Policy Exposure

### Added

- Project 44 documentation
- Wildcard-principal public bucket policy
- `0.0.0.0/0` public IP condition analysis
- `ListBucket` and `GetObject` resource mapping
- Placeholder ARN verification warning
- Access Analyzer and Block Public Access follow-up target

---

## `v1.42.0` - S3 ACL Public Bucket Exposure

### Added

- Project 43 documentation
- S3 Block Public Access disabled evidence
- S3 ACL public List and Read evidence
- Object Ownership / ACL risk analysis
- Follow-up dependency for Access Analyzer and Block Public Access labs
- Public S3 exposure remediation recommendations

---

## Roadmap

- [x] Secure root and IAM administrator access
- [x] Enable centralized audit logging
- [x] Build AWS Organizations and security OUs
- [x] Create organization-level guardrails with SCPs
- [x] Configure IAM Identity Center and delegated administration
- [x] Add GuardDuty and Security Hub foundations
- [x] Route Security Hub findings to SNS email with EventBridge
- [x] Add IAM policy-management permissions for Identity Center administrators
- [x] Protect IdentityCenterAdministration with a permissions boundary
- [x] Explore and delete the default VPC
- [x] Build a custom VPC with public subnets and Internet Gateway routing
- [x] Add private subnets and NAT Gateway egress
- [x] Recreate network with CloudFormation
- [x] Create VPC security groups and security group references
- [x] Launch private EC2 instance with Session Manager
- [x] Add VPC endpoints for private Systems Manager access
- [x] Configure Session Manager Run As and CLI access
- [x] Enable Session Manager S3 logging
- [x] Validate GuardDuty SSH brute-force finding
- [x] Explore access key exposure and static credential risk
- [x] Compare IMDSv1 and IMDSv2 metadata credential exposure
- [x] Explore EC2 user data secret exposure
- [x] Simulate user-data cryptomining behavior and validate GuardDuty
- [x] Create and share forensic EBS snapshot
- [x] Attach forensic volume and analyze mounted snapshot evidence
- [x] Create controlled public S3 ACL exposure
- [x] Create controlled public S3 bucket-policy exposure
- [x] Enable RCPs and attach S3 Classified Sensitive to Prod OU
- [x] Remove the intentionally broken S3 RCP and replace it with an automation-guardrail foundation
- [x] Enable IAM Access Analyzer for organization external access detection
- [x] Apply S3 Block Public Access controls
- [ ] Validate updated Access Analyzer findings
- [ ] Review and remediate remaining Access Analyzer findings
- [ ] Re-enable and validate S3 Block Public Access remediation
- [ ] Add snapshot-sharing prevention guardrails
- [x] Add organization-wide IMDSv2 enforcement guardrails
- [ ] Re-run the EC2 policy status report after enforcement
- [ ] Add centralized logging account delivery
- [ ] Add VPC Flow Logs
- [x] Create multi-region SecurityAutomation EventBridge buses
- [ ] Forward organization S3 and CloudTrail events into SecurityAutomation
- [ ] Build Lambda autoremediation for sensitive S3 buckets
- [ ] Deploy automation components with StackSets
- [ ] Add incident-response automation

---

## Disclaimer

This is a personal AWS lab portfolio. Some decisions are intentionally cost-controlled for a lab environment and are documented separately from production recommendations. Some projects intentionally create unsafe configurations in empty, controlled lab resources to validate detection and prevention controls.
