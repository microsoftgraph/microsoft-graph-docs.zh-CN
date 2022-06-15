---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37910a4a4869e742f3f9c0e884087c5a327423ab
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098766"
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
        "user@odata.bind": "https://graph.microsoft.com/beta/users('0040b377-61d8-43db-94f5-81374122dc7e')",
    }
}
requestBody.SetAdditionalData(map[string]interface{}{
    "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
}
result, err := graphClient.Teams().Post(requestBody)


```