---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 437415113764226354afeb22440429f3d31f717a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083796"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewGroup()
description := "Group assignable to a role"
requestBody.SetDescription(&description)
displayName := "Role assignable group"
requestBody.SetDisplayName(&displayName)
requestBody.SetGroupTypes( []String {
    "Unified",
}
isAssignableToRole := true
requestBody.SetIsAssignableToRole(&isAssignableToRole)
mailEnabled := true
requestBody.SetMailEnabled(&mailEnabled)
securityEnabled := true
requestBody.SetSecurityEnabled(&securityEnabled)
mailNickname := "contosohelpdeskadministrators"
requestBody.SetMailNickname(&mailNickname)
requestBody.SetAdditionalData(map[string]interface{}{
    "owners@odata.bind":  []String {
        "https://graph.microsoft.com/beta/users/99e44b05-c10b-4e95-a523-e2732bbaba1e",
    }
    "members@odata.bind":  []String {
        "https://graph.microsoft.com/beta/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0",
        "https://graph.microsoft.com/beta/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e",
    }
}
options := &msgraphsdk.GroupsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Groups().Post(options)


```