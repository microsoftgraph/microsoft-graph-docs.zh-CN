---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e79d7f4fbe077be11ffc39ce3569ba6df64ac98
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509115"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var topic = new TeamworkActivityTopic
{
    Source = TeamworkActivityTopicSource.EntityUrl,
    Value = "https://graph.microsoft.com/v1.0/users/{userId}/teamwork/installedApps/{installationId}"
};

var activityType = "taskCreated";

var previewText = new ItemBody
{
    Content = "New Task Created"
};

var templateParameters = new List<KeyValuePair>()
{
    new KeyValuePair
    {
        Name = "taskId",
        Value = "Task 12322"
    }
};

await graphClient.Users["{user-id}"].Teamwork
    .SendActivityNotification(topic,activityType,null,previewText,templateParameters)
    .Request()
    .PostAsync();

```