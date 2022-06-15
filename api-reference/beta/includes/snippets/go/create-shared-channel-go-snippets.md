---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86ef6cf57cf031f97b67e6c7a8d58c037cfe9026
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098762"
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
    SetRoles( []String {
        "owner",
    }
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.aadUserConversationMember",
        "user@odata.bind": "https://graph.microsoft.com/beta/users('7640023f-fe43-gv3f-9gg4-84a9efe4acd6')",
    }
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Channels().Post(requestBody)


```