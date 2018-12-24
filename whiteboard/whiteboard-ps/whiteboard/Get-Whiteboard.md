---
applicable: Microsoft Whiteboard
external help file: WhiteboardAdmin-help.xml
Module Name: WhiteboardAdmin
online version:
schema: 2.0.0
title: Get-Whiteboard
---

# Get-Whiteboard

## SYNOPSIS

Gets one or more Whiteboards from the Microsoft Whiteboard service and returns them as objects.

## SYNTAX

### SingleWhiteboard
```
Get-Whiteboard [-Token <AuthenticationResult>] -UserId <Guid> -WhiteboardId <Guid> [-ForceAuthPrompt]
 [<CommonParameters>]
```

### ForUser
```
Get-Whiteboard [-Token <AuthenticationResult>] -UserId <Guid> [-ForceAuthPrompt] [<CommonParameters>]
```

## DESCRIPTION

Gets one or more Whiteboards from the Microsoft Whiteboard service and returns them as objects.

## EXAMPLES

### EXAMPLE 1

```
PS C:\>Get-Whiteboard -UserId 00000000-0000-0000-0000-000000000001
```

Get all of a user's Whiteboards.

## PARAMETERS

### -Token
The Azure AD bearer token corresponding to the specified credentials. If unspecified, a new token will be generated.

```yaml
Type: AuthenticationResult
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserId
Optional. The ID of the user account to query Whiteboards for. All Whiteboards this account has access to will be returned. 

```yaml
Type: Guid
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhiteboardId

Optional. The ID of a specific Whiteboard.

```yaml
Type: Guid
Parameter Sets: SingleWhiteboard
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ForceAuthPrompt

Optional. Always prompt for auth. Use to ignore cached credentials.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: false
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

For details on user IDs, see the [overview page](whiteboard.md).

## RELATED LINKS

## RELATED LINKS
