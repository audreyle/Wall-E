---
title: "Building Secure Azure Cloud Apps"
layout: post
---
This assumes that you understand subscription-based access control roles and how to unlock Resource Groups Names with Microsoft's Managed Identity Service (MIS). 

## Tip 1: Hackers love to scan for secrets that you store in your code. 

Change KeyVault-secret-uri

Use KeyVaultClient.AuthenticationCallBack  
If you are doing this from your local machine, it can either use your identity or your app identity. 

AADManager.FetchSecret

## Tip 2: A great teaching tool for engineers provides them with a way to explore controls instead of getting told "use https only."

Go to Github: AZSK-DevOpsKit.docs for ARM templates. Download the extension.  

The tool scans resources at runtime holistically (computer-secure) to ensure it's compliant with the SharedAccess protocol, and tells engineers exactly which template is failing or if it's applicable. 

**An application only consists of keyvault, resource group name and data.**

Remember: Automation accounts run in the database.   
Azure storage has a CSV file from which you can copy the recommendations.
