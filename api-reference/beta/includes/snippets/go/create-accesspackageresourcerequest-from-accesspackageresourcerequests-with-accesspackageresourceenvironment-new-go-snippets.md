---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ea17d2e49202da1b5123761485c33e488ae0568
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326794"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessPackageResourceRequest()
catalogId := "de9315c1-272b-4905-924b-cc112ca180c7"
requestBody.SetCatalogId(&catalogId)
accessPackageResource := msgraphsdk.NewAccessPackageResource()
requestBody.SetAccessPackageResource(accessPackageResource)
displayName := "Community Outreach"
accessPackageResource.SetDisplayName(&displayName)
description := "https://contoso.sharepoint.com/sites/CSR"
accessPackageResource.SetDescription(&description)
resourceType := "SharePoint Online Site"
accessPackageResource.SetResourceType(&resourceType)
originId := "https://contoso.sharepoint.com/sites/CSR"
accessPackageResource.SetOriginId(&originId)
originSystem := "SharePointOnline"
accessPackageResource.SetOriginSystem(&originSystem)
accessPackageResourceEnvironment := msgraphsdk.NewAccessPackageResourceEnvironment()
accessPackageResource.SetAccessPackageResourceEnvironment(accessPackageResourceEnvironment)
originId := "https://contoso-admin.sharepoint.com/"
accessPackageResourceEnvironment.SetOriginId(&originId)
requestType := "AdminAdd"
requestBody.SetRequestType(&requestType)
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageResourceRequests().Post(requestBody)


```