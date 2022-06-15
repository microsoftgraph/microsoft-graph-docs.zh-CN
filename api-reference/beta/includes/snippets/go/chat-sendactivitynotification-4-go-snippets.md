---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6b2d69abe196df3b90b34b3da2b1976f0e4a0ec
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098752"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
topic := msgraphsdk.NewTeamworkActivityTopic()
requestBody.SetTopic(topic)
source := "entityUrl"
topic.SetSource(&source)
value := "https://graph.microsoft.com/beta/chats/19:1c3af46e9e0f4a5293343c8813c47619@thread.v2"
topic.SetValue(&value)
activityType := "taskCreated"
requestBody.SetActivityType(&activityType)
previewText := msgraphsdk.NewItemBody()
requestBody.SetPreviewText(previewText)
content := "New Task Created"
previewText.SetContent(&content)
recipient := msgraphsdk.NewTeamworkNotificationRecipient()
requestBody.SetRecipient(recipient)
recipient.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.chatMembersNotificationRecipient",
    "chatId": "19:1c3af46e9e0f4a5293343c8813c47619@thread.v2",
}
requestBody.SetTemplateParameters( []KeyValuePair {
    msgraphsdk.NewKeyValuePair(),
name := "taskId"
    SetName(&name)
value := "Task 12322"
    SetValue(&value)
}
chatId := "chat-id"
graphClient.ChatsById(&chatId).SendActivityNotification(chat-id).Post(requestBody)


```