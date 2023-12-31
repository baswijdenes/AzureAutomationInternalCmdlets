---
external help file: Orchestrator.AssetManagement.Cmdlets.dll-Help.xml
Module Name: Orchestrator.AssetManagement.Cmdlets
online version:
schema: 2.0.0
---

# Get-SoftwareUpdateConfigurationMachines

## SYNOPSIS

Retrieves machines associated with an Azure Automation software update configuration.

## SYNTAX

```powershell
Get-SoftwareUpdateConfigurationMachines -SoftwareUpdateConfigurationName <String>
 -SoftwareUpdateConfigurationRunId <Guid> [-ShouldResolveStaticMachines <Boolean>]
 [-StaticMachinesGroupNameToIdMap <String>] [<CommonParameters>]
```

## DESCRIPTION

The `Get-SoftwareUpdateConfigurationMachines` cmdlet is used to retrieve machines associated with an Azure Automation software update configuration. This cmdlet allows you to get information about the machines that are part of a specific software update configuration run, including the ability to resolve static machines and provide a mapping for static machines' group names to IDs.

## EXAMPLES

### Example 1

```powershell
PS C:\> Get-SoftwareUpdateConfigurationMachines -SoftwareUpdateConfigurationName "MySoftwareUpdateConfig" -SoftwareUpdateConfigurationRunId 12345678-90ab-cdef-1234-567890abcdef
```

## PARAMETERS

### -ShouldResolveStaticMachines

Specifies whether to resolve static machines' group names to IDs.

```yaml
Type: Boolean
Parameter Sets: (All)
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
Parameter Sets: (All)
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
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -StaticMachinesGroupNameToIdMap

Provides a mapping of static machines' group names to IDs.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters

This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

System.String

System.Guid

System.Boolean

## OUTPUTS

System.Management.Automation.PSObject

## NOTES

Generated by Bas Wijdenes

## RELATED LINKS

[Bas Wijdenes](https://www.baswijdenes.com)
