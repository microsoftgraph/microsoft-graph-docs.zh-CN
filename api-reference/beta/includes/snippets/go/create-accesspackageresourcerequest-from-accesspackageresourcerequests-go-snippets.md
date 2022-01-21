---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60c8ccae3a816345f487e571472d5f99036797d7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62119057"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessPackageResourceRequest()
catalogId := "26ac0c0a-08bc-4a7b-a313-839f58044ba5"
requestBody.SetCatalogId(&catalogId)
requestType := "AdminAdd"
requestBody.SetRequestType(&requestType)
justification := ""
requestBody.SetJustification(&justification)
accessPackageResource := msgraphsdk.NewAccessPackageResource()
requestBody.SetAccessPackageResource(accessPackageResource)
displayName := "Sales"
accessPackageResource.SetDisplayName(&displayName)
description := "https://contoso.sharepoint.com/sites/Sales"
accessPackageResource.SetDescription(&description)
url := "https://contoso.sharepoint.com/sites/Sales"
accessPackageResource.SetUrl(&url)
resourceType := "SharePoint Online Site"
accessPackageResource.SetResourceType(&resourceType)
originId := "https://contoso.sharepoint.com/sites/Sales"
accessPackageResource.SetOriginId(&originId)
originSystem := "SharePointOnline"
accessPackageResource.SetOriginSystem(&originSystem)
options := &msgraphsdk.AccessPackageResourceRequestsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageResourceRequests().Post(options)


```