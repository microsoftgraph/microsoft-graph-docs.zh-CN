---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e29bed5e4c03fa92fe58d2e02edf3cdabc346656
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60993735"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewChat()
chatType := "oneOnOne"
requestBody.SetChatType(&chatType)
requestBody.SetMembers( []ConversationMember {
    msgraphsdk.NewConversationMember(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.aadUserConversationMember",
        "roles":  []String {
            "owner",
        }
        "user@odata.bind": "https://graph.microsoft.com/v1.0/users('jacob@contoso.com')",
    }
    msgraphsdk.NewConversationMember(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.aadUserConversationMember",
        "roles":  []String {
            "owner",
        }
        "user@odata.bind": "https://graph.microsoft.com/v1.0/users('alex@contoso.com')",
    }
}
options := &msgraphsdk.ChatsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Chats().Post(options)


```