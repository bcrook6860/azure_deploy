CLI commands to the Deploy Control_M VM. Copy and past AS-IS to the Jenkins build.

az group create --name projectctlmrg --location westus
az group deployment create --name projectctlmvm --resource-group projectctlmrg --template-file /home/sbuxproject/azure_deploy/Template_ctlm.vm/ctlm_vm.json --parameters @/home/sbuxproject/azure_deploy/Template_ctlm.vm/ctlm_vm_parameters.json
