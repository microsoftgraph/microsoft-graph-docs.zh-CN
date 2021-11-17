---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e599242e3ebda4f59891ce81ad4b42af42e8dce9
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60990363"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewChannel()
membershipType := "private"
requestBody.SetMembershipType(&membershipType)
displayName := "My First Private Channel"
requestBody.SetDisplayName(&displayName)
description := "This is my first private channels"
requestBody.SetDescription(&description)
requestBody.SetMembers( []ConversationMember {
    msgraphsdk.NewConversationMember(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.aadUserConversationMember",
        "user@odata.bind": "https://graph.microsoft.com/beta/users('jacob@contoso.com')",
        "roles":  []String {
            "owner",
        }
    }
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#Microsoft.Graph.channel",
}
options := &msgraphsdk.ChannelsRequestBuilderPostOptions{
    Body: requestBody,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Channels().Post(options)


```