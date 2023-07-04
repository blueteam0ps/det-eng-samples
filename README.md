# Background
<div class="clear"></div>
<div class="pull-right"><img src="https://raw.githubusercontent.com/blueteam0ps/det-eng-samples/8ccc69bf3ce335447c7a7dc96c17ba8939207896/testing.png" /></div>

This repository exists to support fellow threat detection engineers by providing sample data sets. The sample data sets were created by simulated activity within the Microsoft 365 platform. Simulations were performed via PowerShell using MS API and the M365 web portal. Microsoft Extractor Suite was used to extract the logs for this project. https://github.com/invictus-ir/Microsoft-Extractor-Suite.

# Current Sample Set
                    
No  | Activity | MITRE Tactic | MITRE Technique | MITRE Sub-Technique| Source |  Atomic Red Team Test
-------------  | ------------- |-------------|-------------|-------------|-------------|-------------|
1  | [Password Spraying and followed by a success - MSOLSPRAY](https://raw.githubusercontent.com/blueteam0ps/det-eng-samples/main/dataset/t1110.003_msolspraywithsuccess_1.csv) | TA0006-Credential Access |T1110 | T1110.003| AzureActiveDirectoryStsLogon |
2  | Password Spraying and followed by a success - o365spray(default module) | TA0006-Credential Access | T1110 | T1110.003 | AzureActiveDirectoryStsLogon | 
3  | [Password Spraying and followed by a success - o365spray(reporting module)](https://raw.githubusercontent.com/blueteam0ps/det-eng-samples/main/dataset/t1110.003_o365spray_reporting.csv) | TA0006-Credential Access | T1110 | T1110.003 | AzureActiveDirectoryStsLogon |
4  | [Use MFASweep to identify MFA status of MS Services](https://raw.githubusercontent.com/blueteam0ps/det-eng-samples/main/dataset/t1592.004_mfa_sweep.csv)| TA0043-Reconnaissance | T1592 | T1592.004 | AzureActiveDirectoryStsLogon ||
5  | [Discovery using Azurehound list](https://raw.githubusercontent.com/blueteam0ps/det-eng-samples/main/dataset/t1482_azurehound_list.csv) | TA0007-Discovery | T1482 | - | AzureActiveDirectoryStsLogon | |
6  | [Set Audit Bypass For a Mailbox](https://raw.githubusercontent.com/blueteam0ps/det-eng-samples/main/dataset/t1562-Set-MailboxAuditBypassAssociation.json) | TA0005-Defense Evasion | T1562 | T1562.008 | ExchangeAdmin | |
7  | [Set Mailbox Audit Log Age to Zero](https://raw.githubusercontent.com/blueteam0ps/det-eng-samples/main/dataset/t1562_Set-Mailbox-AuditLogAgeLimitoZero.json)  | TA0005-Defense Evasion | T1562 | T1562.001 | ExchangeAdmin | |
8  | [Disable Unified Audit Log ingestion](https://raw.githubusercontent.com/blueteam0ps/det-eng-samples/main/dataset/t1562-UnifiedAuditlogIngestion-Stopped.json) | TA0005-Defense Evasion | T1562 | T1562.008 | ExchangeAdmin | |
9  | [Assign Company Administrator role to a user in Azure](https://raw.githubusercontent.com/blueteam0ps/det-eng-samples/main/dataset/t1098.001_Add%20a%20user%20to%20company%20administrator%20role.csv) | TA0003-Persistence | T1098 | T1098.001 | Azure Active Directory | |
10 | [Enable IMAP or POP for a mailbox](https://raw.githubusercontent.com/blueteam0ps/det-eng-samples/main/dataset/t1114.002_Enable_POP_IMAP_OWA.csv) | TA0009-Collection | T1114| T1114.002 | ExchangeAdmin | |
11 | [Create external forward a mailbox](https://raw.githubusercontent.com/blueteam0ps/det-eng-samples/main/dataset/t1114_Set-Mailbox-ForwardSMTPAddress.csv) | TA0009-Collection | T1114 | T1114.003 | ExchangeAdmin | 
12 | [Update an existing inbox rule](https://raw.githubusercontent.com/blueteam0ps/det-eng-samples/main/dataset/t1564.008_Update%20existing%20mailbox%20rule%20using%20Set-InboxRule.csv) | TA0005-Defense Evasion | T1564 | T1564.008 | ExchangeAdmin | 
13 | [Set a new inbox rule to delete e-mail](https://raw.githubusercontent.com/blueteam0ps/det-eng-samples/main/dataset/t1564.008_New%20inbox%20rule%20to%20delete%20email.csv) | TA0005-Defense Evasion | T1564 | T1564.008 | ExchangeAdmin | 
14 | [Mailbox delegation with full access](https://raw.githubusercontent.com/blueteam0ps/det-eng-samples/main/dataset/t1098.002_Mail%20Account%20Delegation%20full%20access%20permissions.csv) | TA0003-Persistence | T1098 | T1098.002 | ExchangeAdmin | 
15 | [Mailbox delegation with send as permission](https://raw.githubusercontent.com/blueteam0ps/det-eng-samples/main/dataset/t1098.002_Mail%20account%20delegation-SendAs%20permission.csv) | TA0003-Persistence | T1098 | T1098.002 | ExchangeAdmin | 
16 | [Disable MFA for a user](https://raw.githubusercontent.com/blueteam0ps/det-eng-samples/main/dataset/t1556_Disable%20_Strong_Authentication.json) | TA0003-Persistence | T1556 | T1556.006 | Azure Active Directory | 
17 | [Add ApplicationImpersonation role to an app](https://raw.githubusercontent.com/blueteam0ps/det-eng-samples/main/dataset/t1098.002_ApplicationImpersonation.csv) | TA0003-Persistence | T1098 | T1098.002 | ExchangeAdmin | 
18 | [User removed from an admin group](https://raw.githubusercontent.com/blueteam0ps/det-eng-samples/main/dataset/t1531_Remove-Admin%20members%20from%20a%20group.csv) | TA0040-Impact | T1531 | - | Azure Active Directory | 
19 | [Remove Auditing license from a user](https://raw.githubusercontent.com/blueteam0ps/det-eng-samples/main/dataset/t1562.008_Advanced%20Auditing%20policy%20removed%20from%20a%20user.csv) | TA0005-Defense Evasion | T1562 | T1562.008 | Azure Active Directory |
20 | [Remove of a DLP Compliance Policy](https://raw.githubusercontent.com/blueteam0ps/det-eng-samples/main/dataset/t1562.001_Remove-DlpCompliancePolicy.csv) | TA0005-Defense Evasion | T1562 | T1562.001 | Security Compliance Center | 
21 | [Change Consent Permission to allow any user to allow app grants](https://raw.githubusercontent.com/blueteam0ps/det-eng-samples/main/dataset/t1550.001_Allusers_consent_to_grant_permission_granted.json) | TA0005-Defense Evasion | T1550 | T1550.001 | Azure Active Directory | 
22 | [App Registration for Rclone default config](https://raw.githubusercontent.com/blueteam0ps/det-eng-samples/main/dataset/t1550.001_default_rclone_app_registration.json) | TA0005-Defense Evasion | T1550 | T1550.001 | Azure Active Directory | 


Icon for the project
<a href="https://www.flaticon.com/free-icons/software-testing" title="software testing icons">Software testing icons created by Freepik - Flaticon</a>
