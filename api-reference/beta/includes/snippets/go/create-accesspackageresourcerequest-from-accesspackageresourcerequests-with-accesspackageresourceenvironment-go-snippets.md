---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5be2400c8a178ad9bc6b99e3c59a58dc9b7f17eb
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60983250"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
    "accessPackageResourceEnvironment@odata.bind": "accessPackageResourceEnvironments/615f2218-678f-471f-a60a-02c2f4f80c57",
}
requestType := "AdminAdd"
requestBody.SetRequestType(&requestType)
options := &msgraphsdk.AccessPackageResourceRequestsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageResourceRequests().Post(options)


```