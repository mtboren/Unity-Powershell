---
external help file: Unity-Powershell-help.xml
online version: https://github.com/equelin/Unity-Powershell
schema: 2.0.0
---

# Get-UnityBasicSystemInfo

## SYNOPSIS
Queries the EMC Unity array to retrieve basic informations about arrays.

## SYNTAX

### ByName (Default)
```
Get-UnityBasicSystemInfo [-session <Object>] [-Name <String[]>]
```

### ByID
```
Get-UnityBasicSystemInfo [-session <Object>] [-ID <String[]>]
```

## DESCRIPTION
Queries the EMC Unity array to retrieve basic informations about arrays.
You need to have an active session with the array.

## EXAMPLES

### -------------------------- EXEMPLE 1 --------------------------
```
Get-UnityBasicSystemInfo
```

Retrieve basic information about arrays

## PARAMETERS

### -session
Specifies an UnitySession Object.

```yaml
Type: Object
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: ($global:DefaultUnitySession | where-object {$_.IsConnected -eq $true})
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Specifies the object name.

```yaml
Type: String[]
Parameter Sets: ByName
Aliases: 

Required: False
Position: Named
Default value: *
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -ID
Specifies the object ID.

```yaml
Type: String[]
Parameter Sets: ByID
Aliases: 

Required: False
Position: Named
Default value: *
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES
Written by Erwan Quelin under MIT licence - https://github.com/equelin/Unity-Powershell/blob/master/LICENSE

## RELATED LINKS

[https://github.com/equelin/Unity-Powershell](https://github.com/equelin/Unity-Powershell)

