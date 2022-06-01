---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0cd632a4a6e08bb42037e9530dcb250199f12850
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819843"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var topic = new TeamworkActivityTopic
{
    Source = TeamworkActivityTopicSource.EntityUrl,
    Value = "https://graph.microsoft.com/beta/appCatalogs/teamsApps/{teamsAppId}"
};

var activityType = "pendingFinanceApprovalRequests";

var previewText = new ItemBody
{
    Content = "Internal spending team has a pending finance approval requests"
};

var recipients = new List<TeamworkNotificationRecipient>()
{
    new AadUserNotificationRecipient
    {
        UserId = "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    new AadUserNotificationRecipient
    {
        UserId = "ab88234e-0874-477c-9638-d144296ed04f"
    },
    new AadUserNotificationRecipient
    {
        UserId = "01c64f53-69aa-42c7-9b7f-9f75195d6bfc"
    }
};

var templateParameters = new List<KeyValuePair>()
{
    new KeyValuePair
    {
        Name = "pendingRequestCount",
        Value = "5"
    }
};

await graphClient.Teamwork
    .SendActivityNotificationToRecipients(topic,activityType,null,previewText,null,templateParameters,recipients)
    .Request()
    .PostAsync();

```