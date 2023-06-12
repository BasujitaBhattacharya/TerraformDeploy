# TerraformDeployDemo

## Getting started

## Azure DevOps pipeline

Install the [Terraform extension for Azure DevOps](https://marketplace.visualstudio.com/items?itemName=ms-devlabs.custom-terraform-tasks).

You can also install it from DevOps Organisation Settings > Extensions > Browse Marketplace > Search for Terraform > Install the microsoft provided extension.
![image](https://github.com/BasujitaBhattacharya/TerraformDeployDemo/assets/121059306/f2c12303-6517-4cb4-af5c-4a97250498af)

Create a Service Connection of type Azure Resource Manager at subscription scope. Name the Service Connection `TerraformSvcConn`.
Allow all pipelines to use the connection.

The Pipelines will require the following storage account configurations created in Azure to save the Terraform state:
  
  Storage Account Resource Group: 'rg-terraform-state'
 
  Back end storage account name: 'stracctstate'
  
  Blob storage Container name : 'tfstate'
  
  Back end Storage Key: 'devpipeline.terraform.tfstate'

Back end Storage Key is the name of configuration that will be added to the blob storage account.
Initially the blob container will be empty, once the deploy pipelines run, terrraform state files will be created inside the blob container.

# PublicDevOps
Public repo for files related to Azure DevOps Videos

# Azure DevOps and Bicep Pipelines
Files used for Azure DevOps and Bicep Pipelines Video
https://youtu.be/Q2HZdwTAWG0

# Azure DevOps and Terraform Pipelines
Files used for Azure DevOps and Terraform Pipelines Video
https://youtu.be/d85-KD9stqc

# Image Builder Pipeline
Files used for Azure DevOps and Image Builder
https://youtu.be/zL0eLEl2BxI

# Session Host Pipeline
Files used to deploy Session Hosts with Azure Devops
https://youtu.be/bZy6Yay0ybM

# RestartandUpdateCustomization.txt
Resources for the Image Builder deployment template to add the restart and update customization. 

Files in this repo are for meant as examples and for demonstration purposes only.
