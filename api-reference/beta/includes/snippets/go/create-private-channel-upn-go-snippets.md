---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5eb7d4faae16304cae339ed7b6298bb77639d4a7
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098761"
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
        "user@odata.bind": "https://graph.microsoft.com/beta/users('jacob@contoso.com')",
    }
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#Microsoft.Graph.channel",
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Channels().Post(requestBody)


```