---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e07834e66a4e4fb77973e3a7f3a717a220b99265
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098710"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTeam()
displayName := "My Sample Team"
requestBody.SetDisplayName(&displayName)
description := "My Sample Team’s Description"
requestBody.SetDescription(&description)
requestBody.SetMembers( []ConversationMember {
    msgraphsdk.NewConversationMember(),
    SetRoles( []String {
        "owner",
    }
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.aadUserConversationMember",
        "user@odata.bind": "https://graph.microsoft.com/v1.0/users('0040b377-61d8-43db-94f5-81374122dc7e')",
    }
}
requestBody.SetAdditionalData(map[string]interface{}{
    "template@odata.bind": "https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
}
result, err := graphClient.Teams().Post(requestBody)


```