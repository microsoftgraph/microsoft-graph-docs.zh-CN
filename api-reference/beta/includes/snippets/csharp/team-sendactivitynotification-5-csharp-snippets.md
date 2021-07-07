---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82278c5f9a2d4dd243d47b175c7b83a7cec94d7a
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317125"
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

var recipient = new ChannelMembersNotificationRecipient
{
    TeamId = "e8bece96-d393-4b9b-b8da-69cedef1a7e7",
    ChannelId = "19:3d61a2309f094f4a9310b20f1db37520@thread.tacv2"
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