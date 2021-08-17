---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 772b25d65681a822d6fee1bd8af8a243a19ab778f32ec13ebc7e90edea90a5b6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106747"
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