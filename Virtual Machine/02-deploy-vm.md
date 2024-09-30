# Deploy Azure VM using Arm templates

### Create resource group if it does not exist 

```
az group create --name BroaderAI --location eastus
```

### Create virtual machine

Switch to the folder where you have the `02-create-vm.json` file available.

```
az deployment group create --resource-group broaderAI --template-file 02-create-vm.json
```
