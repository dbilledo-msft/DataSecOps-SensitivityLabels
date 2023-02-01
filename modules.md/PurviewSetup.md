# Module 00 - Lab Environment Setup

**[Home](../README.md)** - [Next Module >](../modules.md/module01.md)

## :loudspeaker: Introduction

In order to follow along with the Microsoft Purview lab exercises, you need to provision a set of resources.

## :thinking: Prerequisites

* An [Azure account](https://azure.microsoft.com/free/) with an active subscription.
* Owner permissions within a Resource Group to create resources and manage role assignments.
* The subscription must have the following resource providers registered.
    * Microsoft.Authorization
    * Microsoft.DataFactory
    * Microsoft.EventHub
    * Microsoft.KeyVault
    * Microsoft.Purview
    * Microsoft.Storage
    * Microsoft.Sql
    * Microsoft.Synapse
    * Microsoft.Insights

## :test_tube: Lab Environment Setup

1. Beneath the **Resource group** field, click **Create new** and provide a unique name (e.g. `purviewlab-rg`), select a [valid location](https://azure.microsoft.com/global-infrastructure/services/?products=purview&regions=all) (e.g. `West Europe`), and then click **Review + create**.

    ![Deploy Template](../images/module00/00.01-deploy-lab.png)

2. Once the validation has passed, click **Create**.

    ![Create Resources](../images/module00/00.02-deploy-create.png)

3. The deployment should take approximately 10 minutes to complete. Once you see the message **Your deployment is complete**, click **Go to resource group**.

    ![Deployment Complete](../images/module00/00.03-deploy-complete.png)

4. If successful, you should see a set of 15 resources, similar to the screenshot below.

    ![Resource Group](../images/module00/00.04-deploy-resources.png)

Note: The Microsoft Purview account resource has been purposely **excluded** from the template so that participants have an opportunity to understand how to deploy a Microsoft Purview account via the Azure Portal.

## :tada: Summary

By successfully deploying the Microsoft Purview lab template, you have the Azure resources needed to follow along with the learning exercises.

[Continue >](../modules.md/module01.md)
