CLI commands to the deploy Oracle VM. Copy and past AS-IS to the Jenkins build.

az group create --name projectorarg --location westus
az group deployment create --name projectoravm --resource-group projectorarg --template-file /home/sbuxproject/azure_deploy/Template_ora.vm/ora_vm.json --parameters @/home/sbuxproject/azure_deploy/Template_ora.vm/ora_vm_parameters.json
