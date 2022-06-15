---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ea8d07cb016f8c86e3c7d2af2befc840cc3eff5
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098755"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
topic := msgraphsdk.NewTeamworkActivityTopic()
requestBody.SetTopic(topic)
source := "entityUrl"
topic.SetSource(&source)
value := "https://graph.microsoft.com/v1.0/users/{userId}/teamwork/installedApps/{installationId}"
topic.SetValue(&value)
activityType := "taskCreated"
requestBody.SetActivityType(&activityType)
previewText := msgraphsdk.NewItemBody()
requestBody.SetPreviewText(previewText)
content := "New Task Created"
previewText.SetContent(&content)
requestBody.SetTemplateParameters( []KeyValuePair {
    msgraphsdk.NewKeyValuePair(),
name := "taskId"
    SetName(&name)
value := "Task 12322"
    SetValue(&value)
}
userId := "user-id"
graphClient.UsersById(&userId).Teamwork().SendActivityNotification(user-id).Post(requestBody)


```