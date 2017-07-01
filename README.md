CLI commands to create the IMS VMs.  Copy and past AS-IS to the Jenkins build.

az group create --name projectvmrg --location "West US"
az group deployment create --name projectvm --resource-group projectvmrg --template-file /home/sbuxproject/azure_deploy/Template_ims.vm/ims_vm.json --parameters @/home/sbuxproject/azure_deploy/Template_ims.vm/ims_vm_parameters.json
