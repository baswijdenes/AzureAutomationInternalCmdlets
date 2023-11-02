---
external help file: Orchestrator.AssetManagement.Cmdlets.dll-Help.xml
Module Name: Orchestrator.AssetManagement.Cmdlets
online version:
schema: 2.0.0
---

# Set-SoftwareUpdateConfigurationRun

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

### Create
```
Set-SoftwareUpdateConfigurationRun -Id <Guid> -SoftwareUpdateConfigurationName <String>
 -ConfiguredDuration <TimeSpan> -OperatingSystem <String> [-Status <String>] -ComputerCount <Int32>
 [-PreScriptSource <String>] [-PostScriptSource <String>] [<CommonParameters>]
```

### Update
```
Set-SoftwareUpdateConfigurationRun -Id <Guid> -Status <String> [-OperationResult <String>] [<CommonParameters>]
```

### UpdatePre
```
Set-SoftwareUpdateConfigurationRun -Id <Guid> -PreScriptJobId <Guid> -PreScriptStatus <String>
 [-OperationResult <String>] [<CommonParameters>]
```

### UpdatePost
```
Set-SoftwareUpdateConfigurationRun -Id <Guid> -PostScriptJobId <Guid> -PostScriptStatus <String>
 [-OperationResult <String>] [<CommonParameters>]
```

### SetTerminalState
```
Set-SoftwareUpdateConfigurationRun -Id <Guid> [-SetTerminalState] [-OperationResult <String>]
 [<CommonParameters>]
```

## DESCRIPTION
{{ Fill in the Description }}

## EXAMPLES

### Example 1
```powershell
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -ComputerCount
{{ Fill ComputerCount Description }}

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
{{ Fill ConfiguredDuration Description }}

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
{{ Fill Id Description }}

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
{{ Fill OperatingSystem Description }}

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
{{ Fill OperationResult Description }}

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
{{ Fill PostScriptJobId Description }}

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
{{ Fill PostScriptSource Description }}

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
{{ Fill PostScriptStatus Description }}

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
{{ Fill PreScriptJobId Description }}

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
{{ Fill PreScriptSource Description }}

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
{{ Fill PreScriptStatus Description }}

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
{{ Fill SetTerminalState Description }}

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
{{ Fill SoftwareUpdateConfigurationName Description }}

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
{{ Fill Status Description }}

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

### System.Guid

### System.String

### System.TimeSpan

### System.Management.Automation.SwitchParameter

### System.Int32

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
