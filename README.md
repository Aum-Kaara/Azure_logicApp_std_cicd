# Azure Logic App Standard CI and CD
Create and deploy a standard logic app using Azure devops 

## Development Environment
* Install .Net Core SDK
* Install Logic App Standard Extention in VS Code 

![image](https://github.com/user-attachments/assets/349a0271-af83-405d-84c7-8a8ab8ca8adc)

* Create a local project

![image](https://github.com/user-attachments/assets/448e0547-5863-4eb1-b44b-8716ff6852bc)

* Browse location and select Statefull and Stateless workflows

![image](https://github.com/user-attachments/assets/d67851e1-ef24-461c-88fb-904455a83c96)

* Create new Resource group

![image](https://github.com/user-attachments/assets/13a6b90b-0fc6-4842-b248-80c8fb1a622e)

Design Logic app with Http trigger and Blob Storage account connection

![image](https://github.com/user-attachments/assets/aed7d514-e0cd-4e2a-b24e-1b18fff2e6df)

![image](https://github.com/user-attachments/assets/78bb6a66-7ea1-4fd4-9034-20ae82b8dcf3)

* Save Logic App

## Create ARM template for Logic App standard 

Link to ARM Template
Link to Parameter File

Use Az cli command to test ARM template 

```
az deployment group create --name ExampleDeployment --resource-group ExampleGroup --template-file storage.json --parameters 'storage.parameters.json'
```

## Create Azure Devops Pipeline

### Build Pipeline for Infra
Create pipeline in Azure Devops to publish artifacts for release(Deploy) pipeline
![image](https://github.com/user-attachments/assets/ea281a74-dd97-44b2-be59-50fe2f435361)

### Create Service Connection 
![image](https://github.com/user-attachments/assets/6ddeebcf-6e80-45b5-a375-d59c3af368c9)

Use service principal automatic 
![image](https://github.com/user-attachments/assets/ad4a48f5-1cb6-4341-9814-3b55d5e0a63a)


### Deploy Pipeline for Infra
Create pipeline in Azure Devops to deploy ARM template to Azure resource group 

![image](https://github.com/user-attachments/assets/126879f8-c9dd-4574-a6d9-b5d35278aad0)

