---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92a810ea12d530ba5a691b311ffee55468fde097
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098670"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
topic := msgraphsdk.NewTeamworkActivityTopic()
requestBody.SetTopic(topic)
source := "entityUrl"
topic.SetSource(&source)
value := "https://graph.microsoft.com/beta/teams/e8bece96-d393-4b9b-b8da-69cedef1a7e7"
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
    "@odata.type": "microsoft.graph.channelMembersNotificationRecipient",
    "teamId": "e8bece96-d393-4b9b-b8da-69cedef1a7e7",
    "channelId": "19:3d61a2309f094f4a9310b20f1db37520@thread.tacv2",
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