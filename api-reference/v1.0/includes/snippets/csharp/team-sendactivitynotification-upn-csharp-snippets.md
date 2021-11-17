---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 741d95ba587adb8271ed55c99fd6265b6f8992ef
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60691585"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var topic = new TeamworkActivityTopic
{
    Source = TeamworkActivityTopicSource.EntityUrl,
    Value = "https://graph.microsoft.com/v1.0/teams/{teamId}/channels/{channelId}/tabs/{tabId}"
};

var activityType = "reservationUpdated";

var previewText = new ItemBody
{
    Content = "You have moved up the queue"
};

var recipient = new AadUserNotificationRecipient
{
    UserId = "jacob@contoso.com"
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
    .SendActivityNotification(topic,activityType,null,previewText,templateParameters,recipient)
    .Request()
    .PostAsync();

```