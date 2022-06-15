---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c40dd3d407c2d66b4f963a292bfcf764a8b2c739
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098732"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewChat()
chatType := "oneOnOne"
requestBody.SetChatType(&chatType)
requestBody.SetMembers( []ConversationMember {
    msgraphsdk.NewConversationMember(),
    SetRoles( []String {
        "owner",
    }
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.aadUserConversationMember",
        "user@odata.bind": "https://graph.microsoft.com/v1.0/users('jacob@contoso.com')",
    }
    msgraphsdk.NewConversationMember(),
    SetRoles( []String {
        "owner",
    }
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.aadUserConversationMember",
        "user@odata.bind": "https://graph.microsoft.com/v1.0/users('alex@contoso.com')",
    }
}
result, err := graphClient.Chats().Post(requestBody)


```