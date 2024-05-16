# Steps to deploy storage account arm template

### Create resource group

```
az group create --name demorg --location 'Central US'
```

### Create the storage account

Switch to the folder where you have the `storage.json` or similar file

```
az deployment group create --resource-group demorg --template-file storage.json
```
