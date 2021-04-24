---
title: How to create a new shared access signature (SAS)
weight: 2
---

# How to create a new shared access signature

## About shared access signatures

A shared access signature (SAS) provides secure delegated access to resources in your storage account. 
With a SAS, you have granular control over how a client can access your data. For example:

 - What resources the client may access
 - What permissions they have to those resources
 - How long the SAS is valid

This page describes how to create a new SAS for your storage container. If you don't have the Azure Blob Container you need to create one. 

[Learn more](https://docs.cloudback.it/how-to/create-microsoft-azure-blob-container/) about how to create a new Azure Blob Container.

## Create a new SAS

To be able to create a new Blob Container it is required to have a storage account. If you don't have a storage account you need to create it first.

 - Open Azure Portal [home page](https://portal.azure.com/#home)
 - Open the storage account page that has the container you want to work with
 - Open page of the container for which you want to create a shared access signature
 - In the left menu click on the `Shared access signature` menu item:
 
<p align="center">
  <img src="https://raw.githubusercontent.com/cloudback/docs/master/static/azure/azure-3-container-page.png" alt="azure container page" title="azure container page" class="screenshot">
</p>

 - Sep up SAS permissions and Start and expiry date/time:

<p align="center">
  <img src="https://raw.githubusercontent.com/cloudback/docs/master/static/azure/azure-4-container-shared-access-signature.png" alt="azure container page" title="azure container page" class="screenshot">
</p>

 - Click on the `Generate SAS token and URL` button
 - After the SAS is generated you will see 'Blob SAS token' and 'Blob SAS URL' are ready to use

<p align="center">
  <img src="https://raw.githubusercontent.com/cloudback/docs/master/static/azure/azure-5-container-shared-access-signature-created.png" alt="azure container page" title="azure container page" class="screenshot">
</p>

Now you can use 'Blob SAS URL' to provide Cloudback access to your own Azure Blob Container. Please note that after the SAS is expired Cloudback will no longer be able to upload backups of your GitHub repositories to your storage.