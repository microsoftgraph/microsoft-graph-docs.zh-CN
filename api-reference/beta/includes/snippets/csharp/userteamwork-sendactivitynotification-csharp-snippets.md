---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 38a29a43969388a2987c9afb7d2e3427e6117fe6168aef25e82c5969d17b746d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216001"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var topic = new TeamworkActivityTopic
{
    Source = TeamworkActivityTopicSource.EntityUrl,
    Value = "https://graph.microsoft.com/beta/users/{userId}/teamwork/installedApps/{installationId}"
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