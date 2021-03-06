---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version: 
schema: 2.0.0
---

# Get-AzureRmApplicationGatewayRequestRoutingRule

## SYNOPSIS
Gets the request routing rule of an application gateway.

## SYNTAX

```
Get-AzureRmApplicationGatewayRequestRoutingRule [-Name <String>] -ApplicationGateway <PSApplicationGateway>
 [<CommonParameters>]
```

## DESCRIPTION
The Get-AzureRmApplicationGatewayRequestRoutingRule cmdlet gets the request routing rule of an application gateway.

## EXAMPLES

### --------------------------  Example 1: Get a specific request routing rule  --------------------------
@{paragraph=PS C:\\\>}





```
PS C:\>$AppGW = Get-AzureRmApplicationGateway -Name "ApplicationGateway01" -ResourceGroupName "ResourceGroup01"
PS C:\> $Rule = Get-AzureRmApplicationGatewayRequestRoutingRule -"Rule01" -ApplicationGateway $AppGW
```

This command gets the request routing rule named Rule01.

### --------------------------  Example 2: Get a list of request routing rules  --------------------------
@{paragraph=PS C:\\\>}





```
PS C:\>$AppGW = Get-AzureRmApplicationGateway -Name "ApplicationGateway01" -ResourceGroupName "ResourceGroup01"
PS C:\> $Rules = Get-AzureRmApplicationGatewayRequestRoutingRule -ApplicationGateway $AppGW
```

This command gets a list of request routing rules.

## PARAMETERS

### -Name
Specifies the name of the request routing rule which this cmdlet gets.

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

### -ApplicationGateway
Specifies the application gateway object that contains request routing rule.

```yaml
Type: PSApplicationGateway
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String

## OUTPUTS

### Microsoft.Azure.Commands.Network.Models.PSApplicationGatewayRequestRoutingRule

### IEnumerable<Microsoft.Azure.Commands.Network.Models.PSApplicationGatewayRequestRoutingRule>

## NOTES
Keywords: azure, azurerm, arm, resource, management, manager, network, networking

## RELATED LINKS

[Add-AzureRmApplicationGatewayRequestRoutingRule]()

[New-AzureRmApplicationGatewayRequestRoutingRule]()

[Remove-AzureRmApplicationGatewayRequestRoutingRule]()

[Set-AzureRmApplicationGatewayRequestRoutingRule]()

