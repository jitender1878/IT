Deploy Azure ARM Template to create multiple VM instances of Windows Server 2019 (max 250). Initial instance set to 3 VM's.

Install Notepad++ to modify template

Create Resource Group ARMTest, VNETARM with Default Subnet to use Parameter File

PowerShell Command without Parameter file

New-AzResourceGroupDeployment –Name TestDeployment –ResourceGroupName ARMTest – TemplateUri https://github.com/jitender1878/IT/blob/main/windowsmultivm-copymethod.json

PowerShell command with Parameter file

New-AzResourceGroupDeployment –Name TestDeployment –ResourceGroupName ARMTest –TemplateUri https://raw.githubusercontent.com/jitender1878/IT/main/windowsmultivm-copymethod.json -TemplateParameterUri https://raw.githubusercontent.com/jitender1878/IT/main/windowsmultivm-parameter.json
