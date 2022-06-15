---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e9214403717e602fd9f628b1495ee190e6459ed
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098667"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
topic := msgraphsdk.NewTeamworkActivityTopic()
requestBody.SetTopic(topic)
source := "entityUrl"
topic.SetSource(&source)
value := "https://graph.microsoft.com/beta/appCatalogs/teamsApps/{teamsAppId}"
topic.SetValue(&value)
activityType := "pendingFinanceApprovalRequests"
requestBody.SetActivityType(&activityType)
previewText := msgraphsdk.NewItemBody()
requestBody.SetPreviewText(previewText)
content := "Internal spending team has a pending finance approval requests"
previewText.SetContent(&content)
requestBody.SetRecipients( []TeamworkNotificationRecipient {
    msgraphsdk.NewTeamworkNotificationRecipient(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a",
    }
    msgraphsdk.NewTeamworkNotificationRecipient(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
        "userId": "ab88234e-0874-477c-9638-d144296ed04f",
    }
    msgraphsdk.NewTeamworkNotificationRecipient(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
        "userId": "01c64f53-69aa-42c7-9b7f-9f75195d6bfc",
    }
}
requestBody.SetTemplateParameters( []KeyValuePair {
    msgraphsdk.NewKeyValuePair(),
name := "pendingRequestCount"
    SetName(&name)
value := "5"
    SetValue(&value)
}
graphClient.Teamwork().SendActivityNotificationToRecipients().Post(requestBody)


```