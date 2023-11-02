---
external help file: Orchestrator.AssetManagement.Cmdlets.dll-Help.xml
Module Name: Orchestrator.AssetManagement.Cmdlets
online version:
schema: 2.0.0
---

# Set-SoftwareUpdateConfigurationMachineRun

## SYNOPSIS

Creates or updates an Azure Automation software update configuration machine run.

## SYNTAX

### Create

```powershell
Set-SoftwareUpdateConfigurationMachineRun -Id <Guid> -SoftwareUpdateConfigurationRunId <Guid> -AgentId <Guid>
 -SoftwareUpdateConfigurationName <String> -TargetComputer <String> -ConfiguredDuration <TimeSpan>
 -OperatingSystem <String> [<CommonParameters>]
```

### Update

```powershell
Set-SoftwareUpdateConfigurationMachineRun -Id <Guid> [-RebootRequired <Boolean>] -Status <String>
 [-EndTime <DateTimeOffset>] [-OperationResult <String>] [<CommonParameters>]
```

## DESCRIPTION

The `Set-SoftwareUpdateConfigurationMachineRun` cmdlet is used to create or update an Azure Automation software update configuration machine run. This cmdlet allows you to configure and manage the properties of machine runs associated with software update configurations.

## EXAMPLES

### Example 1

```powershell
PS C:\> Set-SoftwareUpdateConfigurationMachineRun -Id 12345678-90ab-cdef-1234-567890abcdef -SoftwareUpdateConfigurationRunId 12345678-90ab-cdef-1234-567890abcdef -AgentId 12345678-90ab-cdef-1234-567890abcdef -SoftwareUpdateConfigurationName "MySoftwareUpdateConfig" -TargetComputer "Server01" -ConfiguredDuration 1:00:00 -OperatingSystem "Windows"
```

### Example 2

```powershell
PS C:\> Set-SoftwareUpdateConfigurationMachineRun -Id 12345678-90ab-cdef-1234-567890abcdef -Status "Succeeded"
```

## PARAMETERS

### -AgentId

Specifies the unique identifier (GUID) of the machine agent.

```yaml
Type: Guid
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ConfiguredDuration

Specifies the configured duration for the machine run.

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

### -EndTime

Specifies the end time for the machine run.

```yaml
Type: DateTimeOffset
Parameter Sets: Update
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Id

Specifies the unique identifier (GUID) of the machine run.

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

Specifies the operating system for the machine run.

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

Specifies the operation result for the machine run.

```yaml
Type: String
Parameter Sets: Update
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -RebootRequired

Specifies whether a reboot is required for the machine run.

```yaml
Type: Boolean
Parameter Sets: Update
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -SoftwareUpdateConfigurationName

Specifies the name of the Azure Automation software update configuration.

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

### -SoftwareUpdateConfigurationRunId

Specifies the unique identifier (GUID) of the software update configuration run.

```yaml
Type: Guid
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Status

Specifies the status of the machine run.

```yaml
Type: String
Parameter Sets: Update
Aliases:
Accepted values: NotStarted, InProgress, Succeeded, Failed, MaintenanceWindowExceeded, FailedToStart

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -TargetComputer

Specifies the target computer for the machine run.

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

### CommonParameters

This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

System.Guid

System.String

System.TimeSpan

System.Nullable`1[[System.Boolean, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089]]

System.Nullable`1[[System.DateTimeOffset, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089]]

## OUTPUTS

System.Object

## NOTES

Generated by Bas Wijdenes

## RELATED LINKS

[Bas Wijdenes](https://www.baswijdenes.com)
