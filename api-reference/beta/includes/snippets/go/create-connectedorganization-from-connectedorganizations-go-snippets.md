---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7dae39f3adb18a5e9c62b3f60d332a2bee9630a3
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61005542"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewConnectedOrganization()
displayName := "Connected organization name"
requestBody.SetDisplayName(&displayName)
description := "Connected organization description"
requestBody.SetDescription(&description)
requestBody.SetIdentitySources( []IdentitySource {
    msgraphsdk.NewIdentitySource(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.domainIdentitySource",
        "domainName": "example.com",
        "displayName": "example.com",
    }
}
state := "proposed"
requestBody.SetState(&state)
options := &msgraphsdk.ConnectedOrganizationsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.IdentityGovernance().EntitlementManagement().ConnectedOrganizations().Post(options)


```