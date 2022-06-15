---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2341a875f59a730fc3a943fa5dfc05109ca51a18
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098671"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
topic := msgraphsdk.NewTeamworkActivityTopic()
requestBody.SetTopic(topic)
source := "entityUrl"
topic.SetSource(&source)
value := "https://graph.microsoft.com/beta/teams/{teamId}"
topic.SetValue(&value)
activityType := "pendingFinanceApprovalRequests"
requestBody.SetActivityType(&activityType)
previewText := msgraphsdk.NewItemBody()
requestBody.SetPreviewText(previewText)
content := "Internal spending team has a pending finance approval requests"
previewText.SetContent(&content)
recipient := msgraphsdk.NewTeamworkNotificationRecipient()
requestBody.SetRecipient(recipient)
recipient.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
    "userId": "569363e2-4e49-4661-87f2-16f245c5d66a",
}
requestBody.SetTemplateParameters( []KeyValuePair {
    msgraphsdk.NewKeyValuePair(),
name := "pendingRequestCount"
    SetName(&name)
value := "5"
    SetValue(&value)
}
teamId := "team-id"
graphClient.TeamsById(&teamId).SendActivityNotification(team-id).Post(requestBody)


```