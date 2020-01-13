---
external help file: UniversalAutomation.Cmdlets.dll-Help.xml
Module Name: UniversalAutomation
online version:
schema: 2.0.0
---

# Get-UAJobParameter

## SYNOPSIS
Returns parameters specified for a job.

## SYNTAX

### ById
```
Get-UAJobParameter -JobId <Int64> [-ComputerName <String>] [-AppToken <String>] [<CommonParameters>]
```

### ByObject
```
Get-UAJobParameter -Job <Job> [-ComputerName <String>] [-AppToken <String>] [<CommonParameters>]
```

## DESCRIPTION
Returns parameters specified for a job.

## EXAMPLES

### Example 1
```powershell
PS C:\> Get-UAJobParameter -JobId 10
```

Returns the parameters for job 10.

## PARAMETERS

### -AppToken
An app token to access the UA API. 


```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ComputerName
The HTTP address of the UA REST API server.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Job
The job to return parameters for. 

```yaml
Type: Job
Parameter Sets: ByObject
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -JobId
The job ID to return parameters for. 

```yaml
Type: Int64
Parameter Sets: ById
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

### UniversalAutomation.Job

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
