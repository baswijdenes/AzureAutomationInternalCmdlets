---
external help file: Orchestrator.GraphRunbook.Cmdlets.dll-Help.xml
Module Name: Orchestrator.GraphRunbook.Cmdlets
online version:
schema: 2.0.0
---

# Invoke-RunbookFlow

## SYNOPSIS

Executes a runbook flow using the provided script block nodes.

## SYNTAX

```powershell
Invoke-RunbookFlow -Nodes <ScriptBlock> [<CommonParameters>]
```

## DESCRIPTION

The `Invoke-RunbookFlow` cmdlet is used to execute a runbook flow by specifying a script block containing nodes that define the flow's behavior. The provided script block nodes determine the sequence of activities in the runbook flow.

## EXAMPLES

### Example 1

```powershell
PS C:\> Invoke-RunbookFlow -Nodes {
    Node1 {
        # Define actions for Node1
    }
    Node2 {
        # Define actions for Node2
    }
```

## PARAMETERS

### -Nodes

Specifies a script block containing nodes that define the runbook flow's behavior.

```yaml
Type: ScriptBlock
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters

This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

None

## OUTPUTS

System.Object

## NOTES

Generated by Bas Wijdenes

## RELATED LINKS

[Bas Wijdenes](https://www.baswijdenes.com)
