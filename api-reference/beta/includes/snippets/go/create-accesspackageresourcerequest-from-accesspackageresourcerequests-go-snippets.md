---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93929ffaf51b4f6e83495e424095b2b633964575
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089188"
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
accessPackageResource.SetAdditionalData(map[string]interface{}{
    "displayName": "Sales",
    "description": "https://contoso.sharepoint.com/sites/Sales",
    "url": "https://contoso.sharepoint.com/sites/Sales",
    "resourceType": "SharePoint Online Site",
    "originId": "https://contoso.sharepoint.com/sites/Sales",
    "originSystem": "SharePointOnline",
}
options := &msgraphsdk.AccessPackageResourceRequestsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageResourceRequests().Post(options)


```