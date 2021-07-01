---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94ed5c9c1b1b446bb5f9ef27ff41b0106fd42dd3
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211851"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = new ChatMessage
{
    CreatedDateTime = DateTimeOffset.Parse("2019-02-04T19:58:15.511Z"),
    From = new ChatMessageFromIdentitySet
    {
        User = new Identity
        {
            Id = "8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
            DisplayName = "John Doe"
        }
    },
    Body = new ItemBody
    {
        ContentType = BodyType.Html,
        Content = "Hello World"
    }
};

await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages["{chatMessage-id}"].Replies
    .Request()
    .AddAsync(chatMessage);

```