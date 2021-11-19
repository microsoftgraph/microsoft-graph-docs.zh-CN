---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0241b07667c2cce4630f042c94bfb665cde28e14
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089490"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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