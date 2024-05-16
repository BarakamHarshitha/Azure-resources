# Deploy Azure VM using Arm templates

### Create resource group if it does not exist 

```
az group create --name demorg --location 'Central US'
```

### Create virtual machine

Switch to the folder where you have the `vm.json` file available.

```
az deployment group create --resource-group demorg --template-file vm.json
```
