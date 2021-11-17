---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe1c1296fee5ef1e53ebf634c5b2fc8831d82c8e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61013757"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
topic := msgraphsdk.NewTeamworkActivityTopic()
requestBody.SetTopic(topic)
source := "entityUrl"
topic.SetSource(&source)
value := "https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/tabs/{tabId}"
topic.SetValue(&value)
activityType := "reservationUpdated"
requestBody.SetActivityType(&activityType)
previewText := msgraphsdk.NewItemBody()
requestBody.SetPreviewText(previewText)
content := "You have moved up the queue"
previewText.SetContent(&content)
recipient := msgraphsdk.NewTeamworkNotificationRecipient()
requestBody.SetRecipient(recipient)
recipient.SetAdditionalData(map[string]interface{}{
    "@odata.type": "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient",
    "userId": "569363e2-4e49-4661-87f2-16f245c5d66a",
}
requestBody.SetTemplateParameters( []KeyValuePair {
    msgraphsdk.NewKeyValuePair(),
    SetAdditionalData(map[string]interface{}{
        "name": "reservationId",
        "value": "TREEE433",
    }
    msgraphsdk.NewKeyValuePair(),
    SetAdditionalData(map[string]interface{}{
        "name": "currentSlot",
        "value": "23",
    }
}
options := &msgraphsdk.SendActivityNotificationRequestBuilderPostOptions{
    Body: requestBody,
}
teamId := "team-id"
graphClient.TeamsById(&teamId).SendActivityNotification().Post(options)


```