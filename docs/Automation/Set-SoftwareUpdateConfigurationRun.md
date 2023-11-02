---
external help file: Orchestrator.AssetManagement.Cmdlets.dll-Help.xml
Module Name: Orchestrator.AssetManagement.Cmdlets
online version:
schema: 2.0.0
---

# Set-SoftwareUpdateConfigurationRun

## SYNOPSIS

Sets the configuration for a software update run in Azure Automation.

## SYNTAX

### Create

```powershell
Set-SoftwareUpdateConfigurationRun -Id <Guid> -SoftwareUpdateConfigurationName <String>
 -ConfiguredDuration <TimeSpan> -OperatingSystem <String> [-Status <String>] -ComputerCount <Int32>
 [-PreScriptSource <String>] [-PostScriptSource <String>] [<CommonParameters>]
```

### Update

```powershell
Set-SoftwareUpdateConfigurationRun -Id <Guid> -Status <String> [-OperationResult <String>] [<CommonParameters>]
```

### UpdatePre

```powershell
Set-SoftwareUpdateConfigurationRun -Id <Guid> -PreScriptJobId <Guid> -PreScriptStatus <String>
 [-OperationResult <String>] [<CommonParameters>]
```

### UpdatePost

```powershell
Set-SoftwareUpdateConfigurationRun -Id <Guid> -PostScriptJobId <Guid> -PostScriptStatus <String>
 [-OperationResult <String>] [<CommonParameters>]
```

### SetTerminalState

```powershell
Set-SoftwareUpdateConfigurationRun -Id <Guid> [-SetTerminalState] [-OperationResult <String>]
 [<CommonParameters>]
```

## DESCRIPTION

The `Set-SoftwareUpdateConfigurationRun` cmdlet is used to configure and update a software update run in Azure Automation. It allows you to manage various aspects of the run, including its duration, operating system, scripts, and status.

## EXAMPLES

### Example 1

```powershell
PS C:\> Set-SoftwareUpdateConfigurationRun -Id eeb400b2-9cd3-4370-9a57-45c5b53175df -SoftwareUpdateConfigurationName "UpdateConfig1" -ConfiguredDuration "01:30:00" -OperatingSystem "Windows" -Status "InProgress" -ComputerCount 10
```

## PARAMETERS

### -ComputerCount

Specifies the number of computers involved in the software update run.

```yaml
Type: Int32
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ConfiguredDuration

Specifies the duration of the software update run.

```yaml
Type: TimeSpan
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Id

Specifies the unique ID of the software update run.

```yaml
Type: Guid
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -OperatingSystem

Specifies the target operating system for the software update run.

```yaml
Type: String
Parameter Sets: Create
Aliases:
Accepted values: Windows, Linux

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -OperationResult

Specifies the result of the software update operation.

```yaml
Type: String
Parameter Sets: Update, UpdatePre, UpdatePost, SetTerminalState
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PostScriptJobId

Specifies the unique ID of the post-update script job.

```yaml
Type: Guid
Parameter Sets: UpdatePost
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PostScriptSource

Specifies the source of the post-update script.

```yaml
Type: String
Parameter Sets: Create
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PostScriptStatus

Specifies the status of the post-update script.

```yaml
Type: String
Parameter Sets: UpdatePost
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PreScriptJobId

Specifies the unique ID of the pre-update script job.

```yaml
Type: Guid
Parameter Sets: UpdatePre
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PreScriptSource

Specifies the source of the pre-update script.

```yaml
Type: String
Parameter Sets: Create
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PreScriptStatus

Specifies the status of the pre-update script.

```yaml
Type: String
Parameter Sets: UpdatePre
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -SetTerminalState

Indicates whether to set the terminal state of the software update run.

```yaml
Type: SwitchParameter
Parameter Sets: SetTerminalState
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -SoftwareUpdateConfigurationName

Specifies the name of the software update configuration.

```yaml
Type: String
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Status

Specifies the status of the software update run.

```yaml
Type: String
Parameter Sets: Create
Aliases:
Accepted values: NotStarted, InProgress, Succeeded, Failed, MaintenanceWindowExceeded

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

```yaml
Type: String
Parameter Sets: Update
Aliases:
Accepted values: NotStarted, InProgress, Succeeded, Failed, MaintenanceWindowExceeded

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters

This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

System.Guid

System.String

System.TimeSpan

System.Management.Automation.SwitchParameter

System.Int32

## OUTPUTS

System.Object

## NOTES

Generated by Bas Wijdenes

## RELATED LINKS

[Bas Wijdenes](https://www.baswijdenes.com)
