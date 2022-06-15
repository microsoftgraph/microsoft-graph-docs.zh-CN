---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 91ef95c9880bc013bebfea461d250647c1f0508b
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098711"
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
        "user@odata.bind": "https://graph.microsoft.com/v1.0/users('jacob@contoso.com')",
    }
}
requestBody.SetAdditionalData(map[string]interface{}{
    "template@odata.bind": "https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
}
result, err := graphClient.Teams().Post(requestBody)


```