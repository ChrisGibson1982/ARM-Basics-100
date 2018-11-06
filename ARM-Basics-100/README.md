# Broken deployment of Windows VMs behind a load balancer

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com/ChrisGibson1982/ARM-Basics-100/master/ARM-Basics-100/azuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com/ChrisGibson1982/ARM-Basics-100/master/ARM-Basics-100/azuredeploy.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>

*Example Deployment Command*
New-AzureRmResourceGroupDeployment -Name 'AB100-Deployment' -ResourceGroupName 'AB100-RG' -TemplateUri Https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/101-storage-account-create/azuredeploy.json  -TemplateParameterUri Https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/101-storage-account-create/azuredeploy.parameters.json
