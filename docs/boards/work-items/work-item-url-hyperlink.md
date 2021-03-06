---
title: Define the hyperlink for a work item
titleSuffix: Azure Boards and TFS
description: Construct a URL for a work item for Azure Boards & Team Foundation Server 
ms.prod: devops
ms.technology: devops-agile   
ms.assetid:  
ms.manager: douge
ms.author: kaelli
ms.topic: reference
ms.date: 11/27/2017  
---



# Define the hyperlink for a work item 

[!INCLUDE [temp](../_shared/version-vsts-tfs-all-versions.md)]

You can define the URL for a work item using the syntax provided based on the version or platform you work from. 

Examples in this topic use the following conventions:

-   *OrganizationName* specifies the name of the Azure Boards organization  
-   *ServerName* specifies the name of the TFS application tier server   
-   *Port* specifies the port, default=8080
-   *CollectionName* specifies the name of the project collection.
-   *TeamProjectName* specifies the project name
-   *WorkItemNumber* specifies the ID of the bug, task, or other work item.
 

::: moniker range="vsts"  

<b>https://</b>*OrganizationName.visualstudio.com/ProjectName/*<b>_workitems/edit/</b>*WorkItemNumber*

**Example:** 

```
https://fabrikam/DefaultCollection/Phone%20Saver/_workitems/edit/390
```  

::: moniker-end  

::: moniker range=">= tfs-2015"  

## TFS 2018, TFS 2017, and TFS 2015

<b>http://</b>*ServerName:Port*/<b>tfs/</b>*CollectionName/TeamProjectName*/<b>_workitems?id=</b>*WorkItemNumber*<b>&_a=edit</b>

**Example:** 
```  
http://fabrikamprime:8080/tfs/DefaultCollection/Phone%20Saver/_workitems/133&_a=edit
```  

::: moniker-end  

::: moniker range="tfs-2013"  

## TFS 2013.2

<b>http://</b>*ServerName:Port*/<b>tfs/</b>*CollectionName/TeamProjectName*/<b>_workitems/edit/</b>*WorkItemNumber*

**Example:**
```
http://fabrikamprime:8080/tfs/DefaultCollection/Phone%20Saver/_workitems/edit/133
```

## TFS 2013.1 and earlier versions

<b>http://</b>*ServerName:Port*/<b>tfs/</b>*CollectionName/TeamProjectName*/<b>_workitems#_a=edit&id=</b>*WorkItemNumber*  


**Example:**
```
http://fabrikamprime:8080/tfs/DefaultCollection/Phone%20Saver/_workitems#_a=edit&id=133
```


::: moniker-end  

