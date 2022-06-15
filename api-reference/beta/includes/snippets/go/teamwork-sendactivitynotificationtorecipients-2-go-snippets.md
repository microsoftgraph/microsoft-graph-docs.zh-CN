---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db2d53d3425a3f9fa586c862bd0bde064b41a387
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098666"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
topic := msgraphsdk.NewTeamworkActivityTopic()
requestBody.SetTopic(topic)
source := "text"
topic.SetSource(&source)
value := "Deployment Approvals Channel"
topic.SetValue(&value)
webUrl := "https://teams.microsoft.com/l/message/19:448cfd2ac2a7490a9084a9ed14cttr78c@thread.skype/1605223780000?tenantId=c8b1bf45-3834-4ecf-971a-b4c755ee677d&groupId=d4c2a937-f097-435a-bc91-5c1683ca7245&parentMessageId=1605223771864&teamName=Approvals&channelName=Azure%20DevOps&createdTime=1605223780000"
topic.SetWebUrl(&webUrl)
activityType := "deploymentApprovalRequired"
requestBody.SetActivityType(&activityType)
previewText := msgraphsdk.NewItemBody()
requestBody.SetPreviewText(previewText)
content := "New deployment requires your approval"
previewText.SetContent(&content)
requestBody.SetTemplateParameters( []KeyValuePair {
    msgraphsdk.NewKeyValuePair(),
name := "deploymentId"
    SetName(&name)
value := "6788662"
    SetValue(&value)
}
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
graphClient.Teamwork().SendActivityNotificationToRecipients().Post(requestBody)


```