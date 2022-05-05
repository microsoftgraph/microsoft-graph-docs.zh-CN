---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbb2b73470c4d4fda63354dac40eef5c025cfc69
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202790"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewChannel()
displayName := "My First Shared Channel"
requestBody.SetDisplayName(&displayName)
description := "This is my first shared channel"
requestBody.SetDescription(&description)
membershipType := "shared"
requestBody.SetMembershipType(&membershipType)
requestBody.SetMembers( []ConversationMember {
    msgraphsdk.NewConversationMember(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.aadUserConversationMember",
        "user@odata.bind": "https://graph.microsoft.com/beta/users('7640023f-fe43-gv3f-9gg4-84a9efe4acd6')",
        "roles":  []String {
            "owner",
        }
    }
}
options := &msgraphsdk.ChannelsRequestBuilderPostOptions{
    Body: requestBody,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Channels().Post(options)


```