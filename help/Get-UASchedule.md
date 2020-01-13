---
external help file: UniversalAutomation.Cmdlets.dll-Help.xml
Module Name: UniversalAutomation
online version:
schema: 2.0.0
---

# Get-UASchedule

## SYNOPSIS
Returns schedules defined in UA.

## SYNTAX

### All (Default)
```
Get-UASchedule [-ComputerName <String>] [-AppToken <String>] [<CommonParameters>]
```

### Id
```
Get-UASchedule [-Id] <Int64> [-ComputerName <String>] [-AppToken <String>] [<CommonParameters>]
```

### Identity
```
Get-UASchedule [-Identity] <Identity> [-ComputerName <String>] [-AppToken <String>] [<CommonParameters>]
```

### Script
```
Get-UASchedule [-Script] <Script> [-ComputerName <String>] [-AppToken <String>] [<CommonParameters>]
```

## DESCRIPTION
Returns schedules defined in UA. Schedules define when scripts will be run. 

## EXAMPLES

### Example 1
```powershell
PS C:\> Get-UASchedule
```

Returns all schedules defined in UA. 

### Example 2
```powershell
PS C:\> $Identity = Get-UAIdentity -Name 'Adam'
PS C:\> Get-UASchedule -Identity $Identity
```

Returns all schedules created by the identity 'Adam'

### Example 3
```powershell
PS C:\> $Script = Get-UAScript -Name 'Script.ps1'
PS C:\> Get-UASchedule -Script $Script
```

Returns all schedules for the script 'Script.ps1'

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

### -Id
The ID of the schedule to return.

```yaml
Type: Int64
Parameter Sets: Id
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Identity
The Identity assigned to schedules that should be returned. 

```yaml
Type: Identity
Parameter Sets: Identity
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Script
The script for which their schedules should be returned. 

```yaml
Type: Script
Parameter Sets: Script
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### UniversalAutomation.Identity

### UniversalAutomation.Script

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
