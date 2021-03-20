---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9bedad8f196ff8dc3a0bc2cb6a73d96ff8056caf
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954088"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var topic = new TeamworkActivityTopic
{
    Source = TeamworkActivityTopicSource.EntityUrl,
    Value = "https://graph.microsoft.com/beta/teams/{teamId}"
};

var activityType = "pendingFinanceApprovalRequests";

var previewText = new ItemBody
{
    Content = "Internal spending team has a pending finance approval requests"
};

var recipient = new AadUserNotificationRecipient
{
    UserId = "569363e2-4e49-4661-87f2-16f245c5d66a"
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
    .SendActivityNotification(topic,activityType,null,previewText,templateParameters,recipient,null)
    .Request()
    .PostAsync();

```