---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82c5543d6877c3d7626e213e60410775d2d4d0d1
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098734"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewChannel()
membershipType := "private"
requestBody.SetMembershipType(&membershipType)
displayName := "My First Private Channel"
requestBody.SetDisplayName(&displayName)
description := "This is my first private channels"
requestBody.SetDescription(&description)
requestBody.SetMembers( []ConversationMember {
    msgraphsdk.NewConversationMember(),
    SetRoles( []String {
        "owner",
    }
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.aadUserConversationMember",
        "user@odata.bind": "https://graph.microsoft.com/v1.0/users('62855810-484b-4823-9e01-60667f8b12ae')",
    }
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#Microsoft.Graph.channel",
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Channels().Post(requestBody)


```