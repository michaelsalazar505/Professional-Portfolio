# AWS Cloud Security Engineering Portfolio

> Building a secure AWS environment from the ground up through hands-on cloud security, administration, monitoring, and Infrastructure as Code projects.

**Portfolio Version:** `v1.4.0`  
**Projects Completed:** `5`  
**Status:** Active  
**Last Updated:** July 8, 2026  

---

## Overview

Welcome to the AWS section of my IT Professional Portfolio.

This portfolio documents hands-on projects completed in a personal AWS lab environment. The projects are designed to build practical experience in cloud administration, cloud security, Infrastructure as Code, monitoring, and technical documentation.

Rather than documenting each exercise as a click-by-click lab, every project is presented as a professional engineering case study. Each project explains:

- The problem being solved
- Why the implementation matters
- What was configured
- How the implementation was validated
- What security concepts were demonstrated
- What I learned
- What I would improve in a production environment

The projects build on one another and document the gradual development of a secure AWS security baseline.

---

## Current Portfolio Progress

| # | Project | Document Version | Status | Primary Focus |
|---|---------|------------------|--------|---------------|
| 01 | [Secure AWS Management Account](./01-Secure-AWS-Management-Account/) | `v1.0.1` | ✅ Complete | Root account security and MFA |
| 02 | [Secure IAM Administrator](./02-Secure-IAM-Administrator/) | `v1.0.1` | ✅ Complete | IAM, privileged access, groups, MFA |
| 03 | [CloudTrail Management Event Logging](./03-CloudTrail-Management-Event-Logging/) | `v1.0.1` | ✅ Complete | Audit logging and management-plane visibility |
| 04 | [Multi-Region CloudFormation SecurityAlerts](./04-CloudFormation-SecurityAlerts/) | `v1.0.1` | ✅ Complete | Infrastructure as Code, SNS, multi-region deployment |
| 05 | [Tiered Billing Alerts and Email Notifications](./05-Billing-Alerts-and-SNS-Email/) | `v1.0.0` | ✅ Complete | CloudWatch, billing monitoring, SNS, email alerting |

---

# Security Baseline Built So Far

The first five projects form a connected security foundation.

```text
Project 01
Secure the AWS root identity
        │
        ▼
Project 02
Create a dedicated IAM administrator
        │
        ▼
Project 03
Enable management-plane audit logging
        │
        ▼
Project 04
Build a reusable SecurityAlerts notification foundation with IaC
        │
        ▼
Project 05
Send tiered billing alerts through SecurityAlerts to email
```

This progression demonstrates more than isolated lab completion. It shows the incremental construction of a cloud environment with protected privileged access, audit visibility, repeatable infrastructure deployment, and operational alerting.

---

# Completed Projects

## Project 01 — Secure AWS Management Account

**Version:** `v1.0.1`

Created a dedicated AWS lab account and secured the root identity before deploying additional infrastructure.

### Implemented

- Strong root account password
- Multi-Factor Authentication (MFA)
- Verification that no root access keys were present
- Dedicated account for isolated cloud security lab work

### Skills Demonstrated

- AWS account administration
- Root identity protection
- Privileged credential security
- MFA
- Secure cloud environment preparation

### Why It Matters

The AWS root identity has unrestricted account-level privileges. Securing it first reduces the risk that a single compromised credential could lead to complete account takeover.

---

## Project 02 — Secure IAM Administrator

**Version:** `v1.0.1`

Created a dedicated administrative IAM user so routine administration no longer depended on the AWS root identity.

### Implemented

- Administrators IAM group
- AWS-managed `AdministratorAccess` policy
- Dedicated IAM administrator user
- Group-based permission assignment
- Strong password
- MFA
- Verification that no access keys were present

### Skills Demonstrated

- AWS IAM
- Identity and Access Management
- IAM groups
- AWS managed policies
- MFA
- Privileged access management
- Group-based authorization

### Why It Matters

Separating account ownership from routine administration reduces unnecessary root usage and creates a more manageable access model.

---

## Project 03 — CloudTrail Management Event Logging

**Version:** `v1.0.1`

Configured AWS CloudTrail management-event logging to establish visibility into administrative and API activity.

### Implemented

- Management-event logging
- Logging in `us-west-2`
- Logging in `us-east-2`
- Amazon S3 log delivery
- Cost-conscious lab configuration without a customer-managed KMS key

### Skills Demonstrated

- AWS CloudTrail
- Amazon S3
- Audit logging
- Management-plane visibility
- Multi-region administration
- Cloud governance
- Security monitoring foundations

### Why It Matters

Without management-plane telemetry, it is difficult to determine who changed a resource, which API action occurred, or when an account configuration was modified.

---

## Project 04 — Multi-Region CloudFormation SecurityAlerts

**Version:** `v1.0.1`

Used AWS CloudFormation to deploy identically named `SecurityAlerts` Amazon SNS topics in two AWS regions.

### Implemented

- AWS CloudFormation stack deployment
- Declarative Infrastructure as Code template
- `SecurityAlerts` SNS topic in `us-west-2`
- `SecurityAlerts` SNS topic in `us-east-1`
- Validation of `CREATE_COMPLETE` in both regions
- Multi-region reuse of the same infrastructure definition

### Skills Demonstrated

- AWS CloudFormation
- Infrastructure as Code
- Amazon SNS
- Template review
- Repeatable deployment
- Multi-region provisioning
- Declarative infrastructure

### Why It Matters

Infrastructure as Code provides a repeatable and reviewable way to build consistent infrastructure. The project also created the notification foundation used by later security monitoring projects.

---

## Project 05 — Tiered Billing Alerts and Email Notifications

**Version:** `v1.0.0`

Implemented tiered cost monitoring and linked CloudWatch billing alarms to the existing `SecurityAlerts` SNS topic.

### Implemented

- AWS Free Tier alerts
- CloudWatch billing alerts
- `$10` estimated-charge threshold
- `$25` estimated-charge threshold
- `$50` estimated-charge threshold
- Billing alarms configured in `us-east-1`
- All alarms linked to `SecurityAlerts`
- Confirmed email subscription to the SNS topic

### Skills Demonstrated

- Amazon CloudWatch
- AWS Billing and Cost Management
- Amazon SNS
- CloudWatch alarms
- Cost anomaly awareness
- Notification routing
- Email subscriptions
- Detective security controls

### Why It Matters

Unexpected cloud spending can indicate operational mistakes or suspicious resource usage. Tiered billing alerts create multiple opportunities to detect abnormal cost growth before it becomes a larger problem.

---

# AWS Services Used

The portfolio currently includes hands-on work with:

| Area | Services and Technologies |
|------|---------------------------|
| Identity | AWS IAM, MFA |
| Logging | AWS CloudTrail |
| Storage | Amazon S3 |
| Infrastructure as Code | AWS CloudFormation |
| Notifications | Amazon SNS |
| Monitoring | Amazon CloudWatch |
| Financial Monitoring | AWS Billing and Cost Management |

---

# Regions Used

| Region | Name | Projects |
|--------|------|----------|
| `us-west-2` | US West (Oregon) | CloudTrail, CloudFormation, SNS |
| `us-east-1` | US East (N. Virginia) | CloudFormation, SNS, CloudWatch billing alarms |
| `us-east-2` | US East (Ohio) | CloudTrail |

---

# Skills Developed

## Cloud Administration

- AWS account provisioning
- Regional service configuration
- Resource validation
- AWS Management Console administration

## Identity and Access Management

- Root identity protection
- IAM users
- IAM groups
- AWS managed policies
- MFA
- Privileged access management

## Logging and Monitoring

- CloudTrail management events
- CloudWatch billing alarms
- EstimatedCharges monitoring
- Tiered alert thresholds
- Audit visibility

## Infrastructure as Code

- CloudFormation stacks
- Declarative templates
- Template review
- Repeatable deployment
- Multi-region provisioning

## Security Operations

- Detective security controls
- Alert routing
- SNS notification architecture
- Email subscriptions
- Cost anomaly awareness

## Documentation

- Technical case studies
- Screenshot evidence
- Architecture diagrams
- Security analysis
- Lessons learned
- Production recommendations
- Version history

---

# Documentation Standard

Every project follows the same portfolio documentation standard.

Each project includes:

1. Cover Page
2. Executive Summary
3. Business Problem
4. Objectives
5. Environment
6. Architecture Diagram, when appropriate
7. Implementation Summary
8. Evidence and Screenshots
9. Security Analysis
10. Lessons Learned
11. Production Improvements
12. Skills Demonstrated
13. Resume Bullet
14. STAR Interview Story
15. Version History
16. References

Every provided screenshot is embedded as project evidence, numbered, captioned, and explained.

---

# Repository Structure

```text
AWS-Cloud-Security/
│
├── README.md
│
├── 01-Secure-AWS-Management-Account/
│   ├── README.md
│   ├── Project_01_Secure_AWS_Management_Account_v1.0.1.pdf
│   └── screenshots/
│
├── 02-Secure-IAM-Administrator/
│   ├── README.md
│   ├── Project_02_AWS_IAM_Administrator_Account_v1.0.1.pdf
│   └── screenshots/
│
├── 03-CloudTrail-Management-Event-Logging/
│   ├── README.md
│   ├── Project_03_AWS_CloudTrail_Multi_Region_Logging_v1.0.1.pdf
│   └── screenshots/
│
├── 04-CloudFormation-SecurityAlerts/
│   ├── README.md
│   ├── Project_04_AWS_CloudFormation_SecurityAlerts_v1.0.1.pdf
│   └── screenshots/
│
├── 05-Billing-Alerts-and-SNS-Email/
│   ├── README.md
│   ├── Project_05_AWS_Billing_Alerts_and_SNS_Email_v1.0.0.pdf
│   └── screenshots/
│
└── Resources/
    ├── Templates/
    ├── Diagrams/
    └── Documentation-Standard/
```

---

# Portfolio Statistics

| Metric | Current |
|--------|--------:|
| Portfolio Version | `v1.4.0` |
| Completed AWS Projects | `5` |
| AWS Services Used | `7` |
| AWS Regions Used | `3` |
| Embedded Project Screenshots | `9` |
| Architecture Diagrams | `3` |
| Project PDFs | `5` |
| Status | Active |

---

# Portfolio Version History

## `v1.4.0` — Tiered Billing Monitoring and Notification Delivery

### Added

- Project 05 documentation
- AWS Free Tier alert configuration
- CloudWatch billing alert configuration
- `$10`, `$25`, and `$50` thresholds
- Integration with the `SecurityAlerts` SNS topic
- Confirmed email notification subscription
- Billing alert architecture documentation

---

## `v1.3.0` — Infrastructure as Code and Security Alert Foundation

### Added

- Project 04 documentation
- AWS CloudFormation
- Multi-region stack deployment
- `SecurityAlerts` SNS topics in `us-west-2` and `us-east-1`
- Infrastructure as Code template documentation
- Multi-region architecture diagram

---

## `v1.2.0` — Audit Logging Foundation

### Added

- Project 03 documentation
- AWS CloudTrail management-event logging
- Amazon S3 log delivery
- Multi-region logging configuration
- Cloud audit and governance analysis

---

## `v1.1.0` — Delegated AWS Administration

### Added

- Project 02 documentation
- Dedicated IAM administrator
- Administrators IAM group
- `AdministratorAccess` policy
- MFA for privileged administration
- Group-based permission management

---

## `v1.0.0` — AWS Security Foundation Begins

### Added

- AWS portfolio initialized
- Project 01 documentation
- Dedicated AWS lab account
- Root account password security
- Root MFA
- Verification that no root access keys were present

---

# Roadmap

## Identity and Access

- [x] Secure root account
- [x] Create dedicated IAM administrator
- [x] Protect privileged identities with MFA
- [ ] IAM account alias and password policy
- [ ] IAM Access Analyzer
- [ ] IAM Identity Center

## Logging and Monitoring

- [x] CloudTrail management-event logging
- [x] CloudWatch billing alarms
- [ ] CloudWatch log-based security alerts
- [ ] AWS Config
- [ ] Centralized logging

## Security Detection

- [x] Billing anomaly warning thresholds
- [x] SNS email notification delivery
- [ ] Amazon GuardDuty
- [ ] AWS Security Hub
- [ ] Amazon Inspector

## Infrastructure as Code

- [x] CloudFormation template deployment
- [x] Multi-region stack deployment
- [ ] CloudFormation change sets
- [ ] CloudFormation StackSets
- [ ] Terraform

## Networking and Compute

- [ ] Amazon VPC
- [ ] Security Groups
- [ ] Network ACLs
- [ ] Route Tables
- [ ] Amazon EC2 security
- [ ] AWS Systems Manager

## Governance

- [ ] AWS Organizations
- [ ] Service Control Policies
- [ ] Multi-account security architecture

---

# Engineering Philosophy

Every project is approached as if it were being implemented in a professional environment.

The focus is not only on **how** to configure an AWS service, but also on understanding:

- Why the control exists
- What problem it solves
- What risks it helps reduce
- How the service integrates with the rest of the environment
- How the implementation would be improved for production

---

# Continuous Improvement

This is a living engineering portfolio.

As new projects are completed, this README will be updated with:

- New projects
- New AWS services
- New skills
- Updated architecture diagrams
- Additional evidence
- Version history
- Resume accomplishments
- Interview examples

The goal is to maintain a long-term record of practical cloud engineering and security development.

---

# Disclaimer

This repository documents work completed in a personal AWS lab environment for educational and professional development purposes.

Sensitive information such as account identifiers, email addresses, ARNs, stack identifiers, operation identifiers, and other confidential values is redacted before publication.

Where projects are inspired by structured training, the implementation evidence, analysis, architecture diagrams, lessons learned, and portfolio documentation are presented as my own record of the work I completed and the concepts I learned.
