---
external help file: WssCmdlets.dll-Help.xml
online version: 
schema: 2.0.0
title: Get-WssBackupSystemRecovery
description: 
keywords: powershell, cmdlet
author: andreabarr
manager: jasgro
ms.date: 2017-12-05
ms.topic: reference
ms.prod: powershell
ms.technology: powershell
ms.assetid: CB510903-AAE1-4B1E-B16A-95EEA8F684AF
ms.author: v-anbarr
ms.reviewer: brianlic
---

# Get-WssBackupSystemRecovery

## SYNOPSIS
Gets a bare metal restore option from a scheduled backup policy.

## SYNTAX

```
Get-WssBackupSystemRecovery [-BackupPolicy] <ScheduledBackupPolicy> [<CommonParameters>]
```

## DESCRIPTION
The **Get-WssBackupSystemRecovery** cmdlet gets a value that indicates whether a backup policy can perform bare metal restore operations.
It gets this value from a scheduled backup policy.
A bare metal restore operation restores a full operating system, including critical volumes, from a backup.

## EXAMPLES

### Example 1: Get bare metal restore options from a backup policy
```
PS C:\> Get-WssBackupSystemRecovery -BackupPolicy $ContosoBUPolicy25
```

This command gets the bare metal restore option from the scheduled backup policy that is stored in the variable named **$ContosoBUPolicy25**.

## PARAMETERS

### -BackupPolicy
Specifies the scheduled backup policy for which to display information.

```yaml
Type: ScheduledBackupPolicy
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.WindowsServerSolutions.DataProtection.ServerBackup.ObjectModel.ScheduledBackupPolicy

## OUTPUTS

### System.Boolean
This cmdlet indicates whether BMR is enabled.

## NOTES

## RELATED LINKS

[Add-WssBackupSystemRecovery](./Add-WssBackupSystemRecovery.md)

[Remove-WssBackupSystemRecovery](./Remove-WssBackupSystemRecovery.md)

