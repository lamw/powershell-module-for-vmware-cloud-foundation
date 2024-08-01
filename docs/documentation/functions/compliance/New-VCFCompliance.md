# New-VCFCompliance

## Synopsis

Performs a new VCF compliance audit

## Syntax

```powershell
New-VCFCompliance [-ResourceType] <String> [-StandardType] <String> [-StandardVersion] <String> [-WorkloadDomainName] <String>  [<CommonParameters>]
```

## Description

The `New-VCFWorkloadDomain` cmdlet performs a new VCF compliance audit

## Examples

### Example 1

```powershell
New-VCFCompliance -ResourceType "SDDC_MANAGER" -StandardType "PCI" -StandardVersion "4.0" -WorkloadDomainName "vcf-m01"
```

This example shows how to perform a VCF new compliance audit

## Parameters

### -ResourceType

Resource type for the compliance audit. Please use `Get-VCFComplianceConfiguration` to see available options

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

### -StandardType

Compliance type for the compliance audit. Please use `Get-VCFComplianceStandard` to see available options

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

### -StandardVersion

Compliance version for the compliance audit. Please use `Get-VCFComplianceStandard` to see available options

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

### -WorkloadDomainName

Name of a VCF Management or Workload Domain

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

### Common Parameters

This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).
