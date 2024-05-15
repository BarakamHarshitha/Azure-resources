#login into the Azure 
...
az login
...

# Create VM using Azure CLI
### Start with creating a Resource Group

```
az group create --name learn --location eastus
```

### Set the Resource Group as default (Optional)

```
az config set defaults.group=learn
```

### Create VM with Vnet

```
az vm create \
  --resource-group learn \
  --name learnvm \ 
  --image Ubuntu2204 \
  --vnet-name learnvnet \  
  --subnet learnsubnet \    
  --generate-ssh-keys \
  --output json \
  --verbose
```

### Delete the Resource Group to delete all the resources

```
az group delete --name learn
```
