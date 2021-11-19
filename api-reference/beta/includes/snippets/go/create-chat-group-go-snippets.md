---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f62ec0ae59a6ef33eef20c3fcebf70a8e6ab744
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099232"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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
        "user@odata.bind": "https://graph.microsoft.com/beta/users('8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca')",
    }
    msgraphsdk.NewConversationMember(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.aadUserConversationMember",
        "roles":  []String {
            "owner",
        }
        "user@odata.bind": "https://graph.microsoft.com/beta/users('82fe7758-5bb3-4f0d-a43f-e555fd399c6f')",
    }
    msgraphsdk.NewConversationMember(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.aadUserConversationMember",
        "roles":  []String {
            "owner",
        }
        "user@odata.bind": "https://graph.microsoft.com/beta/users('3626a173-f2bc-4883-bcf7-01514c3bfb82')",
    }
}
options := &msgraphsdk.ChatsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Chats().Post(options)


```