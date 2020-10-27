Easily swap between your Azure subscriptions (updated 2019 Sept)
================================================================

            

Do you manage more than a single Azure subscription and want an easy way to swap between them ?


This function is short and easy to use for anyone.


Step 1


**# install the azure module (one time)**


 


install-module az -force


 


**# run this one time**


 


Enable-AzContextAutosave


login-azaccount


** *** *


**# run this one time**



Get-AzSubscription | fl Name,ID,Tenantid,State


- copy the output from the above command into the different sections from the downloaded function that represent your subscriptions.


Step 2


- You just need to create the hashtables with the Name, ID, TenantID into the function.


Step 3


- Update your validate set on the shortcut names for your subscriptions


 Then you should be ready to go, save and load the function


Step 4


**# will prompt you to login the first time**


azl -account MSDN -auth


**# once you are logged in just swap between accounts**


azl -account PROD


**# once you are logged in just swap between accounts with positional params**



azl PREPROD** *** *



azl MSDN** *** *** *** *


 


 

 

        
    
TechNet gallery is retiring! This script was migrated from TechNet script center to GitHub by Microsoft Azure Automation product group. All the Script Center fields like Rating, RatingCount and DownloadCount have been carried over to Github as-is for the migrated scripts only. Note : The Script Center fields will not be applicable for the new repositories created in Github & hence those fields will not show up for new Github repositories.
