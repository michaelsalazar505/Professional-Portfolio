AWS Cloud Security Engineering Portfolio

Projects Completed: 51
Owner: Michael Salazar
Status: Active / In Progress

Portfolio Summary

This repository documents a hands-on AWS cloud security lab portfolio. The work progresses from account hardening and identity foundations into AWS Organizations, logging, delegated administration, threat detection, alerting, advanced IAM guardrails, cloud networking, Infrastructure as Code, workload-level network security, private compute administration, private AWS service access, SSH replacement with AWS Systems Manager Session Manager, auditable Session Manager logging, exposure-driven GuardDuty detection, static credential risk, EC2 Instance Metadata Service credential exposure, EC2 user data secret exposure, GuardDuty cryptomining detection, EBS snapshot-based cloud forensics, and S3 public access misconfiguration analysis.

The first fifty-one projects form a connected security foundation, now forwarding selected S3 CloudTrail configuration events from the production OU into centralized multi-region SecurityAutomation event buses.

Architecture Progression

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
        |
        v
Project 50 - CloudFormation StackSets Security Event Forwarder Role
        |
        v
Project 51 - StackSets and EventBridge S3 Security Triggers

Completed Projects

#

Project

Status

Focus

01

Secure AWS Management Account

Complete

Root account hardening, MFA, no root access keys

02

Secure IAM Administrator Account

Complete

IAM admin user, Administrators group, MFA, no access keys

03

CloudTrail Management Event Logging

Complete

Multi-region CloudTrail management event logging

04

CloudFormation SecurityAlerts Topic

Complete

SNS topic deployment with CloudFormation

05

Billing Alerts and SNS Email

Complete

Tiered billing alerts and email notification

06

EC2 IAM Role for Systems Manager

Complete

EC2 trust policy and SSM managed instance role

07

CloudTrail S3 ReadWrite IAM Policy

Complete

Customer-managed policy for CloudTrail S3 object access

08

AWS Organizations Security OU and SecurityAudit Account

Complete

Organization, Security OU, and SecurityAudit member account

09

Service Control Policy Guardrails

Complete

Root restriction and organization-leave prevention SCP

10

Cross-Account Role Assumption and Logging Bucket

Complete

OrganizationAccountAccessRole and centralized S3 bucket creation

11

Centralized Logging Bucket Policy

Complete

Restricted CloudTrail bucket/resource policy

12

Organization CloudTrail to SecurityAudit Bucket

Complete

Organization trail redirected to centralized logging storage

13

IAM Identity Center SSO and MFA Foundation

Complete

IAM Identity Center, MFA, admin group, SSO user

14

AdministratorAccess Permission Set Assignment

Complete

AdministratorAccess permission set and SSO admin access validation

15

Enterprise AWS Organizations OU Structure

Complete

Infrastructure, Workloads, Exceptions, Sandbox, Onboarding, Nursery, Suspended, IncidentResponse OUs

16

SCP Target Rework and LogArchive Recovery

Complete

OU guardrail repair, root recovery, LogArchive rename, SecurityAudit recreation

17

RegionLockout SCP

Complete

Region restriction to approved regions and global-service exceptions

18

S3 Lifecycle Cost Control for CloudTrail Logs

Complete

90-day lifecycle expiration for lab cost control

19

Button Up Organization Contacts and Workload OUs

Complete

Trusted access, alternate contacts, Prod/Non-Prod OUs, TestAccount1

20

Delegated Administration for IAM Identity Center and CloudTrail

Complete

IAM delegated admin for Identity Center and SecurityAudit delegated admin for CloudTrail

21

Security Team Permission Sets in IAM Identity Center

Complete

Security Administrators, IAM Administrators, ReadOnlyAccess, IdentityCenterAdmin, SecurityFullAdmin

22

Multi-Region GuardDuty Delegated Administration

Complete

GuardDuty in us-west-2 and us-east-1 with SecurityAudit delegated admin

23

Security Hub Central Configuration

Complete

Security Hub delegated admin, central configuration, standards disabled

24

EventBridge Security Hub Alerts to SNS Email

Complete

SecurityHubFindings rule to SecurityHubAlerts SNS email

25

IAM Identity Center Manage Policies Permission Set

Complete

Policy-management permissions for Identity Center administrators

26

IAM Identity Center Permissions Boundary

Complete

SSOPermissionBoundary and self-escalation control

27

Default VPC Exploration and Cleanup

Complete

Default VPC, subnets, route table, Internet Gateway, deletion after testing

28

Custom VPC Public Subnets and Internet Gateway Routing

Complete

CloudSLAW VPC, public subnets, Internet Gateway, default route

29

Private Subnets and NAT Gateway Egress

Complete

Private subnets, NAT Gateway, private route table, outbound-only Internet access, cleanup

30

CloudFormation VPC Infrastructure as Code

Complete

YAML template, full VPC stack, dependency flowchart, stack validation, stack deletion

31

VPC Security Groups and Security Group References

Complete

Database and Backup security groups, CIDR rules, NFS security-group reference, cleanup

32

Private EC2 Instance with Session Manager

Complete

Amazon Linux EC2, private subnet, SSMClient instance profile, Session Manager access, cleanup

33

Private Subnet Access with VPC Endpoints

Complete

Interface endpoints for ssm, ssmmessages, and ec2messages, private Session Manager access, cleanup

34

Session Manager Run As and CLI Access

Complete

Run As ec2-user, SLAW/SLAW2 instances, AWS CLI start-session, SSH replacement pattern

35

Session Manager S3 Logging

Complete

S3 session logging, SSMLogs inline policy, downloaded command log validation, cleanup

36

GuardDuty Public SSH Exposure

Complete

Public SSH exposure, GuardDuty finding validation, redacted alert evidence, stack cleanup

37

Access Key Exposure and Static Credentials

Complete

AKIA stack, IAM access key creation/deletion, exposed credentials in .aws profile, cleanup

38

IMDSv1 and IMDSv2 Metadata Credential Risk

Complete

IMDS stack, IMDSv1 credential retrieval, IMDSv2 token requirement, SSRF risk analysis, cleanup

39

EC2 User Data Secret Exposure

Complete

SLAW stack, dummy secrets in user data, IMDSv2 retrieval, CloudTrail sensitiveDataRemoved evidence, cleanup

40

User Data Cryptomining GuardDuty Detection

Complete

cloud-init callback to defunct mining domain, GuardDuty HIGH finding validation, cleanup

41

EBS Forensic Snapshot and Cross-Account Sharing

Complete

CSI stack, Hacked volume snapshot, CSI-Incident-1, shared with SecurityAudit

42

Forensics Volume Snapshot Analysis

Complete

SecurityAudit Forensics stack, create CSI volume from shared snapshot, attach and mount volume, recover embedded evidence

43

S3 ACL Public Bucket Exposure

Complete

Block Public Access disabled, ACLs enabled, Everyone List and Read permissions, Access Analyzer follow-up target

44

S3 Misconfigured Bucket Policy Exposure

Complete

Public ListBucket/GetObject through wildcard principal and 0.0.0.0/0 bucket-policy statements

45

S3 Resource Control Policy Prod Guardrail

Superseded - Removed in Project 49

Enabled RCPs, created S3 Classified Sensitive, attached to Prod OU, intentionally broken deny behavior

46

IAM Access Analyzer Delegated External Access

Complete - Findings Review Pending

SecurityAudit delegated admin, organization external analyzers, 17 active resources, email notification

47

S3 Block Public Access Bucket and Account Controls

Complete - Analyzer Validation Pending

Broad BPA on BP bucket, new-only BPA on SLAW bucket, account-level BPA in SecurityAudit

48

EC2 Declarative Policy IMDSv2 Enforcement

Complete

S3 status-report workflow, EC2 policy enablement, uniform report, IMDSv2 defaults attached to Prod

49

EventBridge Security Automation and Broken RCP Replacement

Complete - Automation Buildout Pending

Removed defective S3 RCP and created SecurityAutomation custom event buses in us-east-1 and us-west-2

50

CloudFormation StackSets Security Event Forwarder Role

Complete

Delegated StackSets administration, service-managed organization deployment, SecurityEventForwarder IAM role

51

StackSets and EventBridge S3 Security Triggers

Complete - Event Validation Pending

Production1, Prod OU deployment, multi-region S3 event forwarding, current CreateBucket/TagResource/UntagResource coverage

Latest Project - Project 51: StackSets and EventBridge S3 Security Triggers

Created a new AWS account named Production1, moved it into the Prod OU, and deployed the service-managed SecOpsEventForwarder StackSet from SecurityOperations to the Prod OU in us-west-2 and us-east-1.

The locally maintained YAML template was updated for current S3 behavior by adding CreateBucket, TagResource, and UntagResource while retaining the original bucket-tagging, bucket-policy, and Block Public Access events.

Implemented

Production1 AWS member account

Prod OU placement

Service-managed CloudFormation StackSet

Prod OU targeting by OU ID

us-west-2 deployment

us-east-1 deployment

s3-bucket-security-monitor EventBridge rule

CloudTrail S3 API event matching

Cross-account forwarding to SecurityAutomation

Existing SecurityEventForwarder IAM role

Added CreateBucket

Added TagResource

Added UntagResource

Automatic deployment for future Prod OU accounts

Why It Matters

This project connects the production OU to the centralized security automation platform. Relevant S3 configuration changes can now be forwarded in near real time to SecurityOperations, where later automation can evaluate sensitive-bucket access and enforce the intended data-perimeter invariant.

AWS Services and Technologies Used

Area

Services and Technologies

Identity

AWS IAM, MFA, IAM Roles, AWS STS, IAM Identity Center, Instance Profiles

Compute

Amazon EC2, Amazon Linux, EC2 User Data, EC2 Instance Metadata Service, EC2 Instance Metadata Defaults

Systems Management

AWS Systems Manager Session Manager, AWS CLI Session Manager access

Logging

AWS CloudTrail, Session Manager S3 logging

Storage

Amazon S3, S3 ACLs, S3 Bucket Policies, S3 Block Public Access, S3 Object Ownership, Amazon EBS, EBS Volumes, EBS Snapshots

Infrastructure as Code

AWS CloudFormation, CloudFormation StackSets, YAML

Notifications

Amazon SNS

Monitoring

Amazon CloudWatch

Financial Monitoring

AWS Billing and Cost Management

Governance

AWS Organizations, Service Control Policies, Resource Control Policies, EC2 Declarative Policies, AWS Account Management

Threat Detection

Amazon GuardDuty, AWS Security Hub, IAM Access Analyzer

Eventing

Amazon EventBridge, cross-account event forwarding, CloudTrail-driven S3 security triggers

Networking

Amazon VPC, VPC Endpoints, AWS PrivateLink, Security Groups, NAT Gateway, Internet Gateway, Route Tables, Elastic IP, Network ACLs, DHCP Options

Cloud Forensics

Cross-account snapshot sharing, volume mounting, Linux file-system analysis

Secrets Management

AWS Secrets Manager and SSM Parameter Store recommended as production alternatives

Regions Used

Region

Name

Portfolio Usage

us-west-2

US West (Oregon)

Primary lab region, CloudTrail, CloudFormation, SNS, GuardDuty, Security Hub, EventBridge, VPC, Security Groups, NAT Gateway, EC2, VPC Endpoints, Session Manager, S3 session logs, IMDS testing, user data testing, EBS snapshots, forensic volumes, S3 ACL testing

us-east-1

US East (N. Virginia)

Billing alarms, CloudFormation, SNS, GuardDuty

us-east-2

US East (Ohio)

CloudTrail

Documentation Standard

Each project PDF follows the same portfolio format: cover page, executive summary, business problem, objectives, environment, architecture/workflow diagram, implementation summary, evidence, security analysis, lessons learned, production improvements, skills, resume bullet, STAR story, version history, and references.

Every provided screenshot is embedded as project evidence, numbered, captioned, and explained. Sensitive account identifiers, resource identifiers, access keys, secret access keys, session tokens, and real credentials are redacted where visible. Public-release PDFs are reviewed before publication so unnecessary account and resource metadata is removed while retaining the technical evidence needed to demonstrate the implementation.

Public Release Sanitization

A PDF-only public-release sanitization review was completed on September 2, 2026. The review focused on credentials, AWS account identifiers, AWS Organizations identifiers, subscription metadata, and unique AWS resource identifiers visible in both document text and embedded screenshots.

The following projects received sanitization-only patch releases:

Project

Public Release

Sanitization Update

11

v1.0.1

Removed the AWS account ID embedded in the centralized logging bucket name from document text and evidence

16

v1.0.1

Removed visible AWS Organizations OU identifiers

22

v1.0.1

Removed AWS account and GuardDuty finding/resource identifiers

24

v1.0.1

Removed remaining SNS subscription-specific identifier data

27

v1.0.1

Removed VPC, subnet, route-table, Internet Gateway, DHCP, and related resource identifiers

28

v1.0.1

Removed the CloudSLAW VPC identifier from subnet-creation evidence

30

v1.0.1

Removed the VPC ID and AWS Owner/Account ID from final VPC evidence

33

v1.0.1

Removed the remaining EC2 instance identifier from private SSM evidence

36

v1.0.4

Removed remaining EC2 instance and security-group identifiers while retaining the previously sanitized alert evidence

These releases are sanitization-only revisions. Project architecture, implementation steps, validation results, lessons learned, and security conclusions were not changed.

Portfolio Metrics

Metric

Current Value

Completed AWS Projects

51

AWS Services / Technologies Used

25

Embedded Project Screenshots

141

Architecture Diagrams

49

Project PDFs

51

Disclaimer

This is a personal AWS lab portfolio. Some decisions are intentionally cost-controlled for a lab environment and are documented separately from production recommendations. Some projects intentionally create unsafe configurations in empty, controlled lab resources to validate detection and prevention controls.
