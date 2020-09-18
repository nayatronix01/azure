# Azure HA using Azure Resource Manager


## WordPress with SQL Replicaton 

[WordPress with SQL Replication](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fazure-quickstart-templates%2Fmaster%2Fwordpress-mysql-replication%2Fazuredeploy.json)  

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


## AKS WordPress

virtual network needs to be created and subnet assigned first as template requests existing (not new) info.

[AKS](https://portal.azure.com/#create/Microsoft.Template/uri/https%3a%2f%2fraw.githubusercontent.com%2fAzure%2fazure-quickstart-templates%2fmaster%2f101-aks-advanced-networking%2fazuredeploy.json)


Click on link above  
Log in to Azure  
Select subscription  
Select Resource Group  
Select Region  
Assign Resource name  
Enter location 
Enter DNS prefix  

To get info below, type in and select Azure Active Directory in search box at top of page, go to App registrations, and add new registration if one does not exist. Click on app and copy object ID. For client secret, select Certificates and Secrets in lef pane and add new client secret. Copy secret.  

Enter Existing Service Principal Object Id  - select Azure Active Directory, users. Select user. Copy Object ID under Identity section  
Enter Existing Service Principal Client Id  - select Azure Active Director, app registrations. add new registration for app. Copy application (client) ID.  
Existing Service Principal Client Secret  - select Certificates and Secrets in lef pane and add new client secret. Copy secret. Only visible on creation so store. 


Select built in role type  
Enter Existing Virtual network name  
enter Existing Virtual Network Resource Group  
Enter Existing subnet name  







