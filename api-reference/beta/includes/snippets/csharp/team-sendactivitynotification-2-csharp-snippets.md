---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e813156d5a59a7f3272c5a069d41cbb78c9b5f69
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573228"
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
    .SendActivityNotification(topic,activityType,null,previewText,templateParameters,recipient)
    .Request()
    .PostAsync();

```