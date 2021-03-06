# Azure WebApp and Private Azure SQL 

Example template to deploy Azure resources to support a WebApp connecting to an Azure SQL Database instance using private networking. 

![webapp private SQL architecture](/static/arch.png)

## ARM Template

The ARM templated in this repo will deploy all required resources for this solution with a baseline configuration. 

Included int he deployment is a management virtual machine and Azure Bastion host for accessing the private Virtual Network. The Azure SQL Database is not accessible over public networks, this VM can be used to access the database instance. 

### Azure Portal

Use the following links to load the ARM template into the Azure portal for easy deployment.

[![Deploy To Azure](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazure.svg?sanitize=true)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fhibbertda%2Faz-webapp-privateSQL%2Fmain%2Ftemplate%2Fazuredeploy.json)
[![Deploy To Azure US Gov](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazuregov.svg?sanitize=true)](https://portal.azure.us/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fhibbertda%2Faz-webapp-privateSQL%2Fmain%2Ftemplate%2Fazuredeploy.json)