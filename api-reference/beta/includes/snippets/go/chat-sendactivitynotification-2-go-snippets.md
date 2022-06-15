---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f89bae2936f862668d5061a0562e16c02df4c7ee
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098750"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
topic := msgraphsdk.NewTeamworkActivityTopic()
requestBody.SetTopic(topic)
source := "entityUrl"
topic.SetSource(&source)
value := "https://graph.microsoft.com/beta/chats/{chatId}/messages/{messageId}"
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
    "userId": "569363e2-4e49-4661-87f2-16f245c5d66a",
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