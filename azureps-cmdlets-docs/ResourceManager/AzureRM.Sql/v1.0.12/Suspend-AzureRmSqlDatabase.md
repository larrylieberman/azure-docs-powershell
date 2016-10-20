---
external help file: Microsoft.Azure.Commands.Sql.dll-Help.xml
online version: .\Get-AzureRmSqlDatabase.md
schema: 2.0.0
ms.assetid: B083D3E9-A931-4793-8B34-3B4FB8D46663
---

# Suspend-AzureRmSqlDatabase

## SYNOPSIS
Suspends a SQL Data Warehouse database.

## SYNTAX

```
Suspend-AzureRmSqlDatabase [-ServerName] <String> -DatabaseName <String> [-ResourceGroupName] <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Suspend-AzureRmSqlDatabase** cmdlet suspends an azure_2 SQL Data Warehouse database.

## EXAMPLES

### Example 1: Suspends an Azure SQL Data Warehouse database
```
PS C:\>Suspend-AzureRmSqlDatabase -ResourceGroupName "ResourceGroup01" -ServerName "Server01" -DatabaseName "Database01"
```

This command suspends an active azure_2 SQL Data Warehouse database.

## PARAMETERS

### -ServerName
Specifies the name of the server which hosts the database.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -DatabaseName
Specifies the name of the database that this cmdlet suspends.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group to which the server is assigned.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -InformationAction
@{Text=}

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
@{Text=}

```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Azure.Commands.Sql.Database.Model.AzureSqlDatabaseModel

## OUTPUTS

### Microsoft.Azure.Commands.Sql.Database.Model.AzureSqlDatabaseModel

## NOTES
* The **Suspend-AzureRmSqlDatabase** cmdlet works only on azure_2 SQL Data Warehouse databases. This operation is not supported on ssSDS Basic, Standard and Premium editions.

## RELATED LINKS

[Get-AzureRmSqlDatabase](.\Get-AzureRmSqlDatabase.md)

[New-AzureRmSqlDatabase](.\New-AzureRmSqlDatabase.md)

[Remove-AzureRmSqlDatabase](.\Remove-AzureRmSqlDatabase.md)

[Resume-AzureRmSqlDatabase](.\Resume-AzureRmSqlDatabase.md)

[Set-AzureRmSqlDatabase](.\Set-AzureRmSqlDatabase.md)

[Azure SQL Database Cmdlets](.\AzureRM.Sql.md)

