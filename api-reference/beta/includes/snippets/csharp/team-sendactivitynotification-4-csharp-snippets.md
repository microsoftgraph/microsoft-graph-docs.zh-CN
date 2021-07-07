---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c57e7b6f56e0662638f3edccb75531683c8363d
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317121"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var topic = new TeamworkActivityTopic
{
    Source = TeamworkActivityTopicSource.EntityUrl,
    Value = "https://graph.microsoft.com/beta/teams/e8bece96-d393-4b9b-b8da-69cedef1a7e7"
};

var activityType = "pendingFinanceApprovalRequests";

var previewText = new ItemBody
{
    Content = "Internal spending team has a pending finance approval requests"
};

var recipient = new TeamMembersNotificationRecipient
{
    TeamId = "e8bece96-d393-4b9b-b8da-69cedef1a7e7"
};

var templateParameters = new List<KeyValuePair>()
{
    new KeyValuePair
    {
        Name = "pendingRequestCount",
        Value = "5"
    }
};

await graphClient.Teams["{team-id}"]
    .SendActivityNotification(topic,activityType,null,previewText,templateParameters,recipient)
    .Request()
    .PostAsync();

```