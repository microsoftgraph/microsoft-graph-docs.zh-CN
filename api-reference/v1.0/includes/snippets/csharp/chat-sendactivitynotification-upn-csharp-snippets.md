---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2af83a30366e407b488acf8842469ea81aad089d
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696494"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var topic = new TeamworkActivityTopic
{
    Source = TeamworkActivityTopicSource.EntityUrl,
    Value = "https://graph.microsoft.com/v1.0/chats/{chatId}/messages/{messageId}"
};

var activityType = "approvalRequired";

var previewText = new ItemBody
{
    Content = "Deployment requires your approval"
};

var recipient = new AadUserNotificationRecipient
{
    UserId = "jacob@contoso.com"
};

var templateParameters = new List<KeyValuePair>()
{
    new KeyValuePair
    {
        Name = "approvalTaskId",
        Value = "2020AAGGTAPP"
    }
};

await graphClient.Chats["{chat-id}"]
    .SendActivityNotification(topic,activityType,null,previewText,templateParameters,recipient)
    .Request()
    .PostAsync();

```