# FIN10
## Description
[[Group/G0051|FIN10]] is a financially motivated threat group that has targeted organizations in North America since at least 2013 through 2016. The group uses stolen data exfiltrated from victims to extort organizations.FireEye FIN10 June 2017
## Attribution
| Tactic | Technique | Tool | Description |
|--------|---------|-------|---------|
| Execution Persistence Privilege Escalation |       Scheduled Task                    |  | [[FIN10]] has established persistence by using S4U tasks as well as the Scheduled Task option in PowerShell Empire.FireEye FIN10 June 2017Github PowerShell Empire |                                                           
| Defense Evasion Execution |                        Scripting                         |  | [[FIN10]] has executed malicious .bat files containing PowerShell commands.FireEye FIN10 June 2017 |                                                                                                                           
| Lateral Movement |                                 Remote Desktop Protocol           |  | [[FIN10]] has used RDP to move laterally to systems in the victim environment.FireEye FIN10 June 2017 |                                                                                                                        
| Defense Evasion Persistence Privilege Escalation | Valid Accounts                    |  | [[FIN10]] has used stolen credentials to connect remotely to victim networks using VPNs protected with only a single factor. The group has also moved laterally using the Local Administrator account.FireEye FIN10 June 2017 |
| Execution |                                        PowerShell                        |  | [[FIN10]] uses PowerShell for execution as well as PowerShell Empire to establish persistence.FireEye FIN10 June 2017Github PowerShell Empire |                                                                                
| Discovery |                                        System Owner/User Discovery       |  | [[FIN10]] has used Meterpreter to enumerate users on remote systems.FireEye FIN10 June 2017 |                                                                                                                                  
| Defense Evasion |                                  File Deletion                     |  | [[FIN10]] has used batch scripts and scheduled tasks to delete critical system files.FireEye FIN10 June 2017 |                                                                                                                 
| Command and Control Lateral Movement |             Remote File Copy                  |  | [[FIN10]] has deployed Meterpreter stagers and SplinterRAT instances in the victim network after moving laterally.FireEye FIN10 June 2017 |                                                                                    
| Persistence |                                      Registry Run Keys / Start Folder  |  | [[FIN10]] has established persistence by using the Registry option in PowerShell Empire to add a Run key.FireEye FIN10 June 2017Github PowerShell Empire |                                                                     



