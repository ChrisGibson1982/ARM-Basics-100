# Broken deployment of Windows VMs behind a load balancer

There are 3 issues with this template that need to be resolved.  All produce error messages.

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com/ChrisGibson1982/ARM-Basics-100/master/ARM-Basics-100/azuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com/ChrisGibson1982/ARM-Basics-100/master/ARM-Basics-100/azuredeploy.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>

## Example PowerShell Deployment Command
New-AzureRmResourceGroupDeployment -Name ExampleDeployment -ResourceGroupName ExampleResourceGroup -TemplateUri https://raw.githubusercontent.com/ChrisGibson1982/ARM-Basics-100/master/ARM-Basics-100/azuredeploy.json  -TemplateParameterUri https://raw.githubusercontent.com/ChrisGibson1982/ARM-Basics-100/master/ARM-Basics-100/azuredeploy.parameters.json

## Example Azure Cli Deployment Command
az account set --subscription 'SUBSCRIPTION NAME'

az group deployment create --resource-group ExampleResourceGroup --template-file azuredeploy.json --parameters azuredeploy.parameters.json
