# Getting Started with Node JS Test application

> [!NOTE]
> Please read and implement [Infrastructure](https://github.com/prashantchamps/sas-test-iac/blob/main/README.md) repository document then continue with this.

## Introduction

This is a demo application build in Reach JS. Here we are going to build image of this application and then push on Azure Container Registry with a GitHub workflow. Packaging of the application is done using yarn. Also a Dockerfile is created to build the image.

## Steps to deploy application on ACR
1) Create below repository level secrets and if you have read [Infrastructure](https://github.com/prashantchamps/sas-test-iac/blob/main/README.md) repository document then get the values from there.
   - AZURE_CLIENT_ID
   - AZURE_CLIENT_SECRET
2) Go to GitHub Actions in this repository and run workflow "Build and Push Image".
   
   > [!NOTE]
   > Currently it is kept as manual run but we can automate it's trigger on push to the codebase.

## How to test
Go to Azure portal and check weather your image is created with proper tag in Azure Container Registry or not.
