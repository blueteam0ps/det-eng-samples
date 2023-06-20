# Background
<div class="clear"></div>
<div class="pull-right"><img src="https://raw.githubusercontent.com/blueteam0ps/det-eng-samples/8ccc69bf3ce335447c7a7dc96c17ba8939207896/testing.png" /></div>

This repository exists to support fellow threat detection engineers by providing sample data sets. The sample data sets were created by simulated activity within the Microsoft 365 platform. Simulations were performed via PowerShell using MS API and the M365 web portal. Microsoft Extractor Suite was used to extract the logs for this project. https://github.com/invictus-ir/Microsoft-Extractor-Suite.

# Current Sample Set
                    
No  | Activity | MITRE Tactic | MITRE Technique | MITRE Sub-Technique| Source | Sample | Atomic Red Team Test
-------------  | ------------- |-------------|-------------|-------------|-------------|-------------|-------------|
1  | Password Spraying and followed by a success - MSOLSPRAY | TA0006-Credential Access |T1110 | T1110.003| AzureActiveDirectoryStsLogon | |
2  | Password Spraying and followed by a success - o365spray(default module) | TA0006-Credential Access | T1110 | T1110.003 | AzureActiveDirectoryStsLogon | |
3  | Password Spraying and followed by a success - o365spray(reporting module) | TA0006-Credential Access | T1110 | T1110.003 | AzureActiveDirectoryStsLogon | |
4  | Use MFASweep to identify MFA status of MS Services | TA0043-Reconnaissance | T1592 | T1592.004 | AzureActiveDirectoryStsLogon | |
5  | Discovery using Azurehound list | TA0007-Discovery | T1482 | - | AzureActiveDirectoryStsLogon | |
6  | Set Audit Bypass For a Mailbox | TA0005-Defense Evasion | T1562 | T1562.008 | ExchangeAdmin | |
7  | Set Mailbox Audit Log Age to Zero  | TA0005-Defense Evasion | T1562 | T1562.001 | ExchangeAdmin | |
8  | Disable Unified Audit Log ingestion | TA0005-Defense Evasion | T1562 | T1562.008 | ExchangeAdmin | |
9  | Assign Company Administrator role to a user in Azure | TA0003-Persistence | T1098 | T1098.001 | Azure Active Directory | |
10 | Enable IMAP or POP for a mailbox | TA0009-Collection | T1114| T1114.002 | ExchangeAdmin | |
11 | Create external forward a mailbox | TA0009-Collection | T1114 | T1114.003 | ExchangeAdmin | 
12 | Update an existing inbox rule | TA0005-Defense Evasion | T1564 | T1564.008 | ExchangeAdmin | 
13 | Set a new inbox rule to delete e-mail | TA0005-Defense Evasion | T1564 | T1564.008 | ExchangeAdmin | 
14 | Mailbox delegation with full access | TA0003-Persistence | T1098 | T1098.002 | ExchangeAdmin | 
15 | Mailbox delegation with send as permission | TA0003-Persistence | T1098 | T1098.002 | ExchangeAdmin | 
16 | Disable MFA for a user | TA0003-Persistence | T1556 | T1556.006 | Azure Active Directory | 
17 | Add ApplicationImpersonation role to an app | TA0003-Persistence | T1098 | T1098.002 | ExchangeAdmin | 
18 | User removed from an admin group | TA0040-Impact | T1531 | - | Azure Active Directory | 
19 | Remove Auditing license from a user | TA0005-Defense Evasion | T1562 | T1562.008 | Azure Active Directory |
20 | Remove of a DLP Compliance Policy | TA0005-Defense Evasion | T1562 | T1562.001 | Security Compliance Center | |

Icon for the project
<a href="https://www.flaticon.com/free-icons/software-testing" title="software testing icons">Software testing icons created by Freepik - Flaticon</a>
