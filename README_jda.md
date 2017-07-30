CLI commands to create the JDA VM. Copy and past AS-IS to the Jenkins build.

az group create --name projectvm2rg --location "West US"
az group deployment create --name projectvm2 --resource-group projectvm2rg --template-file /home/sbuxproject/azure_deploy/Template_jda.vm/jda_vm.json --parameters @/home/sbuxproject/azure_deploy/Template_jda.vm/jda_vm_parameters.json
