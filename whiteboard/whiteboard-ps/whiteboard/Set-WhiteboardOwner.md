---
applicable: Microsoft Whiteboard
external help file: WhiteboardAdmin-help.xml
Module Name: WhiteboardAdmin
online version:
schema: 2.0.0
title: Set-WhiteboardOwner
---

# Set-WhiteboardOwner

## SYNOPSIS

Sets the owner for a Whiteboard.

## SYNTAX

```
Set-WhiteboardOwner [[-Token] <AuthenticationResult>] [-WhiteboardId] <Guid> [-OldOwnerId] <Guid>
 [-NewOwnerId] <Guid> [-ForceAuthPrompt] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION

Sets the owner for a Whiteboard.

## EXAMPLES

### EXAMPLE 1

```
PS C:\>Set-WhiteboardOwner -OldOwnerId 00000000-0000-0000-0000-000000000001 -NewOwnerId 00000000-0000-0000-0000-000000000002
```

Move a Whiteboard from one user to another.

## PARAMETERS

### -Token

The Azure AD bearer token corresponding to the specified credentials. If unspecified, a new token will be generated.

```yaml
Type: AuthenticationResult
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhiteboardId

The Whiteboard for which the owner is being changed.

```yaml
Type: Guid
Parameter Sets: (All)
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OldOwnerId

The ID of the previous owner.

```yaml
Type: Guid
Parameter Sets: (All)
Aliases:

Required: True
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NewOwnerId

The ID of the new owner.

```yaml
Type: Guid
Parameter Sets: (All)
Aliases:

Required: True
Position: 4
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

### -WhatIf

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
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

For details on user IDs, see the [overview page](whiteboard.md).

## RELATED LINKS
