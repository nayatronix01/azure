# Azure HA using Azure Resource Manager

I have used Azure once before and the timeframe for this requirement and getting up to speed with Azure is too short. I investigated and found that Azure Resource manager is used to deploy templates in Azure. The templates below can be used to deploy the services in Azure:  

## WordPress with SQL Replicaton

[WordPress with SQL Replication]

(https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fazure-quickstart-templates%2Fmaster%2Fwordpress-mysql-replication%2Fazuredeploy.json)

Click on link above  
Log into Azure portal

Select subscription  
Select Resource Group  
Select Region  
Assign site name
Assign hosting plan name  (Free, Shared, Basic, Standard)  
Choose SKU 
Assign DNS hostname
Assign Public IP name  
Assign VM username
Assign Mysql root password
Assign Mysql replication password
Assign Mysql proble password  
Select VM size
Assign Virtual network name
Choose whether virtual network name is new or existing  
Enter an existing virtual network Resource Group name  
Assign DB subnet name
Select authentication type

The rest of the options can be left as thtey are or can be changed to suit 
Click on Next:Review + create button 

If validation succeeds, click on create. Otherwise click Previous and correct errors.



[AKS] 
(https://portal.azure.com/#create/Microsoft.Template/uri/https%3a%2f%2fraw.githubusercontent.com%2fAzure%2fazure-quickstart-templates%2fmaster%2f101-aks-advanced-networking%2fazuredeploy.json)
