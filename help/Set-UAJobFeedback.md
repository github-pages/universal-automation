---
external help file: UniversalAutomation.Cmdlets.dll-Help.xml
Module Name: UniversalAutomation
online version:
schema: 2.0.0
---

# Set-UAJobFeedback

## SYNOPSIS
Sets the feedback for a job that has requested it.

## SYNTAX

```
Set-UAJobFeedback -JobFeedback <JobFeedback> [-Response <String>] [-ComputerName <String>] [-AppToken <String>]
 [<CommonParameters>]
```

## DESCRIPTION
Sets the feedback for a job that has requested it. Use Get-UAJobFeedback to retrieve feedback objects for a job. 

## EXAMPLES

### Example 1
```powershell
PS C:\> $Job = Get-UAJob -Id 2
PS C:\> $JobFeedback = Get-UAJobFeedback -Job $Job
PS C:\> Set-UAJobFeedback -JobFeedback $JobFeedback -Response "Hello, world!"
```

Responds to the job feedback with 'Hello, world!'

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

### -JobFeedback
The job feedback to respond to. Use Get-UAJobFeedback to retrieve a JobFeedback object. 

```yaml
Type: JobFeedback
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Response
The reponse to the feedback. 

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
