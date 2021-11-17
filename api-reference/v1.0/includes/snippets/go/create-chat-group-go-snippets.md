---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 53e88c32fa75a704a5daf645f5d0dbd758549b8e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60993734"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewChat()
chatType := "group"
requestBody.SetChatType(&chatType)
topic := "Group chat title"
requestBody.SetTopic(&topic)
requestBody.SetMembers( []ConversationMember {
    msgraphsdk.NewConversationMember(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.aadUserConversationMember",
        "roles":  []String {
            "owner",
        }
        "user@odata.bind": "https://graph.microsoft.com/v1.0/users('8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca')",
    }
    msgraphsdk.NewConversationMember(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.aadUserConversationMember",
        "roles":  []String {
            "owner",
        }
        "user@odata.bind": "https://graph.microsoft.com/v1.0/users('82fe7758-5bb3-4f0d-a43f-e555fd399c6f')",
    }
    msgraphsdk.NewConversationMember(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.aadUserConversationMember",
        "roles":  []String {
            "owner",
        }
        "user@odata.bind": "https://graph.microsoft.com/v1.0/users('3626a173-f2bc-4883-bcf7-01514c3bfb82')",
    }
}
options := &msgraphsdk.ChatsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Chats().Post(options)


```