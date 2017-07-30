CLI commands to create the Control_M VM. Copy and past AS-IS to the Jenkins build.

az group create --name projectvmrg --location "West US"
az group deployment create --name projectvm --resource-group projectvmrg --template-file /home/sbuxproject/azure_deploy/Template_ctl.vm/ctlm_vm.json --parameters @/home/sbuxproject/azure_deploy/Template_ctlm.vm/ctl_vm_parameters.json
