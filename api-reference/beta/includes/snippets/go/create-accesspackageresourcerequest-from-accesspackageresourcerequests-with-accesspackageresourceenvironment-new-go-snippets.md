---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3e38bfe430492c185f9c8f0857c925adf5e303c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096711"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessPackageResourceRequest()
catalogId := "de9315c1-272b-4905-924b-cc112ca180c7"
requestBody.SetCatalogId(&catalogId)
accessPackageResource := msgraphsdk.NewAccessPackageResource()
requestBody.SetAccessPackageResource(accessPackageResource)
accessPackageResource.SetAdditionalData(map[string]interface{}{
    "displayName": "Community Outreach",
    "description": "https://contoso.sharepoint.com/sites/CSR",
    "resourceType": "SharePoint Online Site",
    "originId": "https://contoso.sharepoint.com/sites/CSR",
    "originSystem": "SharePointOnline",
}
requestType := "AdminAdd"
requestBody.SetRequestType(&requestType)
options := &msgraphsdk.AccessPackageResourceRequestsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageResourceRequests().Post(options)


```