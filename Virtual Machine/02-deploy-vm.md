# Deploy Azure VM using Arm templates

### Create resource group if it does not exist 

```
az group create --name broaderAI --location 'Central US'
```

### Create virtual machine

Switch to the folder where you have the `01-create-vm.json` file available.

```
az deployment group create --resource-group broaderAI --template-file 01-create-vm.json
```