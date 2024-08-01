# Get-VCFComplianceTask

## Synopsis

Retrieves the list of all VCF compliance configurations along with their applicable resource types and versions

## Syntax

```powershell
Get-VCFComplianceTask [-WorkloadDomainName] <String> [-ComplianceTaskId] <String> [<CommonParameters>]
```

## Description

The `Get-VCFComplianceTask` cmdlet the compliance audit id and progress using the task Id returned from the `New-VCFCompliance` operation

## Examples

### Example 1

```powershell
Get-VCFComplianceTask -WorkloadDomainName "vcf-m01" -ComplianceTaskId "d22c47e0-8d38-43da-975b-938e7c59f4d6"

id                                   status     complianceAuditId
--                                   ------     -----------------
d22c47e0-8d38-43da-975b-938e7c59f4d6 SUCCESSFUL 1758e972-8509-4dce-93d9-a303d7c35a41
```

This example shows how to retrieve the compliance audit id and progress using the task Id returned from the `New-VCFCompliance` operation

### -WorkloadDomainName

 Name of a VCF Management or Workload Domain

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ComplianceTaskId

Compliance task returned from New-VCFCompliance

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```