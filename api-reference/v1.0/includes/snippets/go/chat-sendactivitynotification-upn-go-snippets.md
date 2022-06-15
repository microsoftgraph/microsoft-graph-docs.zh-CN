---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0018d03577d1e947dd014fe355b11a9ab58250cc
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098784"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
topic := msgraphsdk.NewTeamworkActivityTopic()
requestBody.SetTopic(topic)
source := "entityUrl"
topic.SetSource(&source)
value := "https://graph.microsoft.com/v1.0/chats/{chatId}/messages/{messageId}"
topic.SetValue(&value)
activityType := "approvalRequired"
requestBody.SetActivityType(&activityType)
previewText := msgraphsdk.NewItemBody()
requestBody.SetPreviewText(previewText)
content := "Deployment requires your approval"
previewText.SetContent(&content)
recipient := msgraphsdk.NewTeamworkNotificationRecipient()
requestBody.SetRecipient(recipient)
recipient.SetAdditionalData(map[string]interface{}{
    "@odata.type": "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient",
    "userId": "jacob@contoso.com",
}
requestBody.SetTemplateParameters( []KeyValuePair {
    msgraphsdk.NewKeyValuePair(),
name := "approvalTaskId"
    SetName(&name)
value := "2020AAGGTAPP"
    SetValue(&value)
}
chatId := "chat-id"
graphClient.ChatsById(&chatId).SendActivityNotification(chat-id).Post(requestBody)


```