# Steps to deploy storage account arm template

### Create resource group

```
az group create --name broaderAI --location 'Central US'
```

### Create the storage account

Switch to the folder where you have the `01-storage-account.json` or similar file

```
az deployment group create --resource-group broaderAI --template-file 01-storage-account.json
```