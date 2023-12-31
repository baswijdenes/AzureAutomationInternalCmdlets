---
external help file: Orchestrator.AssetManagement.Cmdlets.dll-Help.xml
Module Name: Orchestrator.AssetManagement.Cmdlets
online version:
schema: 2.0.0
---

# Set-AutomationVariable

## SYNOPSIS

Sets the value of an Azure Automation variable.

## SYNTAX

```powershell
Set-AutomationVariable -Value <Object> [-Name] <String> [<CommonParameters>]
```

## DESCRIPTION

The `Set-AutomationVariable` cmdlet is used to set the value of an Azure Automation variable. Automation variables allow you to store and manage data in your automation environment. You can use this cmdlet to update the value of a specific variable.

## EXAMPLES

### Example 1

```powershell
PS C:\> Set-AutomationVariable -Name "MyVariable" -Value "NewValue"
```

{{ Add example description here }}

## PARAMETERS

### -Name

Specifies the name of the Azure Automation variable to update.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Value

Specifies the name of the Azure Automation variable to update.

```yaml
Type: Object
Parameter Sets: (All)
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

System.Object

System.String

## OUTPUTS

System.Object

## NOTES

Generated by Bas Wijdenes

## RELATED LINKS

[Bas Wijdenes](https://www.baswijdenes.com)
