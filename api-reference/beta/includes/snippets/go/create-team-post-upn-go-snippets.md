---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d10720a40667a558d10bd7a146345cf8cd9a140a
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098767"
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
        "user@odata.bind": "https://graph.microsoft.com/beta/users('jacob@contoso.com')",
    }
}
requestBody.SetAdditionalData(map[string]interface{}{
    "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
}
result, err := graphClient.Teams().Post(requestBody)


```