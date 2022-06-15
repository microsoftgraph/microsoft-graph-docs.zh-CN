---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3d741b6d2f561aad658f1d48d172125c4a9b515
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098751"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
topic := msgraphsdk.NewTeamworkActivityTopic()
requestBody.SetTopic(topic)
source := "entityUrl"
topic.SetSource(&source)
value := "https://graph.microsoft.com/beta/chats/{chatId}"
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
    "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
    "userId": "569363e2-4e49-4661-87f2-16f245c5d66a",
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