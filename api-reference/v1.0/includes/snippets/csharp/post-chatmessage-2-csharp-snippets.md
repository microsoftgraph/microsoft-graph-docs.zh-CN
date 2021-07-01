---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b67e76b874986ab01317d4c41484db210554c84
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207729"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = new ChatMessage
{
    Body = new ItemBody
    {
        ContentType = BodyType.Html,
        Content = "Hello World <at id=\"0\">Jane Smith</at>"
    },
    Mentions = new List<ChatMessageMention>()
    {
        new ChatMessageMention
        {
            Id = 0,
            MentionText = "Jane Smith",
            Mentioned = new ChatMessageMentionedIdentitySet
            {
                User = new Identity
                {
                    DisplayName = "Jane Smith",
                    Id = "ef1c916a-3135-4417-ba27-8eb7bd084193",
                    UserIdentityType = TeamworkUserIdentityType.AadUser
                }
            }
        }
    }
};

await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages
    .Request()
    .AddAsync(chatMessage);

```