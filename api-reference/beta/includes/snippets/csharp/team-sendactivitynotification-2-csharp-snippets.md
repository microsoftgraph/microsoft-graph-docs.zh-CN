---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86adc1cdcc89e181ec5954a6483b469ccdaf9f9d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954096"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var topic = new TeamworkActivityTopic
{
    Source = TeamworkActivityTopicSource.EntityUrl,
    Value = "https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/tabs/{tabId}"
};

var activityType = "reservationUpdated";

var previewText = new ItemBody
{
    Content = "You have moved up the queue"
};

var recipient = new AadUserNotificationRecipient
{
    UserId = "569363e2-4e49-4661-87f2-16f245c5d66a"
};

var templateParameters = new List<KeyValuePair>()
{
    new KeyValuePair
    {
        Name = "reservationId",
        Value = "TREEE433"
    },
    new KeyValuePair
    {
        Name = "currentSlot",
        Value = "23"
    }
};

await graphClient.Teams["{team-id}"]
    .SendActivityNotification(topic,activityType,null,previewText,templateParameters,recipient,null)
    .Request()
    .PostAsync();

```