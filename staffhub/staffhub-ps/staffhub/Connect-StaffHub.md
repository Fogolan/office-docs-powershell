---
applicable: Microsoft StaffHub
external help file: Microsoft.OutlookApps.StaffHub.PowershellCmdlets.dll-Help.xml
Module Name: MicrosoftStaffHub
online version:
schema: 2.0.0
title: Connect-StaffHub
---

# Connect-StaffHub

## SYNOPSIS
The `Connect-StaffHub` cmdlet connects an authenticated account to use for Microsoft StaffHub cmdlet requests.
You can use this authenticated account only with Microsoft StaffHub cmdlets.

Note: The cmdlet is currently in Beta.

## SYNTAX

```
Connect-StaffHub [[-Credentials] <PSCredential>] [[-LogLocation] <String>] [[-LogHistoryInDays] <Int32>]
 [[-CultureInfo] <String>] [<CommonParameters>]
```

## DESCRIPTION
The `Connect-StaffHub` cmdlet connects an authenticated account. This cmdlet authenticates a user for Staff Hub.
You can use this authenticated account only with Microsoft StaffHub cmdlets.

## EXAMPLES

### Example 1
```
Connect-StaffHub -Credentials $mycreds
```

LogIn the session with the specified credential.

### Example 2
```
Connect-StaffHub
```

Prompts to enter credentials and then Log in.

## PARAMETERS

### -Credentials
PSCredential object of the credential.
Eg: $secpasswd = ConvertTo-SecureString "password" -AsPlainText -Force
$mycreds = New-Object System.Management.Automation.PSCredential ("username", $secpasswd)

```yaml
Type: PSCredential
Parameter Sets: (All)
Aliases:

Required: False
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CultureInfo
CultureInfo in which the message is to be displayed.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: en-US
Accept pipeline input: False
Accept wildcard characters: False
```

### -LogHistoryInDays
Number of days the logs are to be persisted.
Default value is 10 days.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: 10
Accept pipeline input: False
Accept wildcard characters: False
```

### -LogLocation
Location where the logs are to be persisted in user's box.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None

## OUTPUTS

### System.Object

## NOTES

The cmdlet is currently in Beta.

## RELATED LINKS

[MicrosoftStaffHub Module in Gallery](https://www.powershellgallery.com/packages/MicrosoftStaffHub/1.0.0-alpha)
