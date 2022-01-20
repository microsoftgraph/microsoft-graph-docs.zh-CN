---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 21f467c9fda7626a0391ab3e2b81409fbcb86634
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62119055"
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
options := &msgraphsdk.AccessPackageResourceRequestsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageResourceRequests().Post(options)


```