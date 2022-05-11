---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ffc819a54fbf72f8e8cab588504ebdb7cb985882
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329237"
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
result, err := graphClient.Groups().Post(requestBody)


```