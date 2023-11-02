# Azure Automation Internal Cmdlets

This document provides information about Azure Automation internal cmdlets.  
The documents are generated with [PlatyPS](https://github.com/PowerShell/platyPS) and the blanks are filled with [ChatGPT](https://chat.openai.com/).  

**Handle the documentation with care. It may be that not everything is correct because the blanks are generated with AI.**

## Automation

- [Get-AutomationCertificate](\docs\Automation\Get-AutomationCertificate.md)
- [Get-AutomationConnection](\docs\Automation\Get-AutomationConnection.md)
- [Get-AutomationPSCredential](\docs\Automation\Get-AutomationPSCredential.md)
- [Get-AutomationVariable](\docs\Automation\Get-AutomationVariable.md)
- [Get-SoftwareUpdateConfigurationMachines](\docs\Automation\Get-SoftwareUpdateConfigurationMachines.md)
- [Initialize-AutomationSoftwareUpdateConfiguration](\docs\Automation\Initialize-AutomationSoftwareUpdateConfiguration.md)
- [Invoke-AutomationWatcherAction](\docs\Automation\Invoke-AutomationWatcherAction.md)
- [Set-AutomationVariable](\docs\Automation\Set-AutomationVariable.md)
- [Set-SoftwareUpdateConfigurationMachineRun](.\docs\Automation\Set-SoftwareUpdateConfigurationMachineRun.md)
- [Set-SoftwareUpdateConfigurationRun](\docs\Automation\Set-SoftwareUpdateConfigurationRun.md)
- [Start-AutomationRunbook](\docs\Automation\Start-AutomationRunbook.md)
- [Wait-AutomationJob](\docs\Automation\Wait-AutomationJob.md)

## RunbookFlow

- [Invoke-RunbookFlow.md](\docs\RunbookFlow\Invoke-RunbookFlow.md)
- [New-RunbookFlowJunction.md](\docs\RunbookFlow\New-RunbookFlowJunction.md)
- [New-RunbookFlowLink.md](\docs\RunbookFlow\New-RunbookFlowLink.md)
- [New-RunbookFlowScript.md](\docs\RunbookFlow\New-RunbookFlowScript.md)
- [Set-RunbookFlowActivityInput.md](\docs\RunbookFlow\Set-RunbookFlowActivityInput.md)

## What are Azure Automation internal cmdlets?

Azure Automation internal cmdlets are cmdlets that you can use within Azure Automation. The most common are Variables, certificates, and credentials.  
These are cmdlets that you can use to call or start information within the Azure Automation environment you are currently working in.  
The advantage of this is that you do not have to log in via `Connect-AzAccount` and provide the resource group and Azure Automation account name, but there are definitely more possibilities with these cmdlets.  

Do you have questions or feedback? You can then submit an issue or adjust or supplement the documentation yourself.
