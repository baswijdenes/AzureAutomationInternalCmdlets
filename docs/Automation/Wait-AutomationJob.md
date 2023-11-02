---
external help file: Orchestrator.AssetManagement.Cmdlets.dll-Help.xml
Module Name: Orchestrator.AssetManagement.Cmdlets
online version:
schema: 2.0.0
---

# Wait-AutomationJob

## SYNOPSIS
{{ Fill in the Synopsis }}

## SYNTAX

```
Wait-AutomationJob -Id <Guid[]> [-TimeoutInMinutes <Int32>] [-DelayInSeconds <Int32>]
 [-OutputJobsTransitionedToRunning] [<CommonParameters>]
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

### -DelayInSeconds
Specifies the time in seconds between retries to retrieve the job status list.
The minimum time between retries is 30 seconds, and the maximum is 300 seconds.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id
Specifies the list of job IDs that can be passed to this cmdlet.
The maximum number of job IDs is 1000.

```yaml
Type: Guid[]
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -OutputJobsTransitionedToRunning
Specifies if the cmdlet outputs Running jobs

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TimeoutInMinutes
Specifies the maximum time in minutes that this cmdlet can run.
The default timeout is 5 minutes.
The maximum allowed is 60 minutes.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.Guid[]

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS