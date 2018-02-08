---
applicable: Exchange Server 2010, Exchange Server 2013, Exchange Server 2016, Exchange Online
schema: 2.0.0
---

# Remove-RetentionPolicyTag

## SYNOPSIS
!!! Exchange Server 2010

Use the Remove-RetentionPolicyTag cmdlet to remove a retention tag.

When you use the Remove-RetentionPolicyTag cmdlet to remove a retention tag, it removes the tag definition stored in Active Directory. The next time the Managed Folder Assistant runs, it processes all items that have the removed tag applied and restamps them. Depending on the number of mailboxes and messages, this process may result in significant resource consumption on all Mailbox servers that contain mailboxes with a retention policy that included the removed tag.

For more information about retention tags, see Understanding Retention Tags and Retention Policies.

!!! Exchange Server 2013, Exchange Server 2016, Exchange Online

This cmdlet is available in on-premises Exchange and in the cloud-based service. Some parameters and settings may be exclusive to one environment or the other.

Use the Remove-RetentionPolicyTag cmdlet to remove a retention tag.

For information about the parameter sets in the Syntax section below, see Exchange cmdlet syntax (https://technet.microsoft.com/library/bb123552.aspx).

## SYNTAX

```
Remove-RetentionPolicyTag [-Identity] <RetentionPolicyTagIdParameter> [-Confirm] [-DomainController <Fqdn>]
 [-WhatIf] [<CommonParameters>]
```

## DESCRIPTION
!!! Exchange Server 2010

Retention tags are added to a retention policy, which is applied to a mailbox.

You need to be assigned permissions before you can run this cmdlet. Although all parameters for this cmdlet are listed in this topic, you may not have access to some parameters if they're not included in the permissions assigned to you. To see what permissions you need, see the "Messaging records management" entry in the Messaging Policy and Compliance Permissions topic.

!!! Exchange Server 2013

Retention tags are added to a retention policy, which is applied to a mailbox.

When you use the Remove-RetentionPolicyTag cmdlet to remove a retention tag, it removes the tag definition stored in Active Directory. The next time the Managed Folder Assistant runs, it processes all items that have the removed tag applied and restamps them. Depending on the number of mailboxes and messages, this process may result in significant resource consumption on all Mailbox servers that contain mailboxes with a retention policy that includes the removed tag.

For more information about retention tags, see Retention tags and retention policies.

You need to be assigned permissions before you can run this cmdlet. Although all parameters for this cmdlet are listed in this topic, you may not have access to some parameters if they're not included in the permissions assigned to you. To see what permissions you need, see the "Messaging records management" entry in the Messaging policy and compliance permissions topic.

!!! Exchange Server 2016, Exchange Online

Retention tags are added to a retention policy, which is applied to a mailbox.

When you use the Remove-RetentionPolicyTag cmdlet to remove a retention tag, it removes the tag definition stored in Active Directory. The next time the Managed Folder Assistant runs, it processes all items that have the removed tag applied and restamps them. Depending on the number of mailboxes and messages, this process may result in significant resource consumption on all Mailbox servers that contain mailboxes with a retention policy that includes the removed tag.

For more information about retention tags, see Retention tags and retention policies in Exchange 2016.

You need to be assigned permissions before you can run this cmdlet. Although this topic lists all parameters for the cmdlet, you may not have access to some parameters if they're not included in the permissions assigned to you. To find the permissions required to run any cmdlet or parameter in your organization, see Find the permissions required to run any Exchange cmdlet (https://technet.microsoft.com/library/mt432940.aspx).

## EXAMPLES

### Example 1 -------------------------- (Exchange Server 2010)
```
Remove-RetentionPolicyTag -Identity "Finance-DeletedItems"
```

This example removes the retention tag Finance-DeletedItems.

### Example 1 -------------------------- (Exchange Server 2013)
```
Remove-RetentionPolicyTag -Identity "Finance-DeletedItems"
```

This example removes the retention tag Finance-DeletedItems.

### Example 1 -------------------------- (Exchange Server 2016)
```
Remove-RetentionPolicyTag -Identity "Finance-DeletedItems"
```

This example removes the retention tag Finance-DeletedItems.

### Example 1 -------------------------- (Exchange Online)
```
Remove-RetentionPolicyTag -Identity "Finance-DeletedItems"
```

This example removes the retention tag Finance-DeletedItems.

## PARAMETERS

### -Identity
The Identity parameter specifies the name of the retention policy tag.

```yaml
Type: RetentionPolicyTagIdParameter
Parameter Sets: (All)
Aliases:
Applicable: Exchange Server 2010, Exchange Server 2013, Exchange Server 2016, Exchange Online

Required: True
Position: 1
Default value: None
Accept pipeline input: True
Accept wildcard characters: False
```

### -Confirm
The Confirm switch specifies whether to show or hide the confirmation prompt. How this switch affects the cmdlet depends on if the cmdlet requires confirmation before proceeding.

- Destructive cmdlets (for example, Remove-\* cmdlets) have a built-in pause that forces you to acknowledge the command before proceeding. For these cmdlets, you can skip the confirmation prompt by using this exact syntax: -Confirm:$false.

- Most other cmdlets (for example, New-\* and Set-\* cmdlets) don't have a built-in pause. For these cmdlets, specifying the Confirm switch without a value introduces a pause that forces you acknowledge the command before proceeding.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:
Applicable: Exchange Server 2010, Exchange Server 2013, Exchange Server 2016, Exchange Online

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DomainController
!!! Exchange Server 2010

The DomainController parameter specifies the domain controller that's used by this cmdlet to read data from or write data to Active Directory. You identify the domain controller by its fully qualified domain name (FQDN). For example, dc01.contoso.com.



!!! Exchange Server 2013, Exchange Server 2016, Exchange Online

This parameter is available only in on-premises Exchange.

The DomainController parameter specifies the domain controller that's used by this cmdlet to read data from or write data to Active Directory. You identify the domain controller by its fully qualified domain name (FQDN). For example, dc01.contoso.com.



```yaml
Type: Fqdn
Parameter Sets: (All)
Aliases:
Applicable: Exchange Server 2010, Exchange Server 2013, Exchange Server 2016, Exchange Online

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
The WhatIf switch simulates the actions of the command. You can use this switch to view the changes that would occur without actually applying those changes. You don't need to specify a value with this switch.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:
Applicable: Exchange Server 2010, Exchange Server 2013, Exchange Server 2016, Exchange Online

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (https://go.microsoft.com/fwlink/p/?LinkID=113216).

## INPUTS

###  
To see the input types that this cmdlet accepts, see Cmdlet Input and Output Types (https://go.microsoft.com/fwlink/p/?LinkId=616387). If the Input Type field for a cmdlet is blank, the cmdlet doesn't accept input data.

## OUTPUTS

###  
To see the return types, which are also known as output types, that this cmdlet accepts, see Cmdlet Input and Output Types (https://go.microsoft.com/fwlink/p/?LinkId=616387). If the Output Type field is blank, the cmdlet doesn't return data.

## NOTES

## RELATED LINKS

[Online Version](https://technet.microsoft.com/library/0db7cb8a-83aa-4843-b7fb-d562b837294a.aspx)
