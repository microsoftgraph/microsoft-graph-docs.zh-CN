---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1aa5ea33d3b02365a554bfb1ebfb5866eaad08a9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964271"
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
            Mentioned = new IdentitySet
            {
                User = new Identity
                {
                    DisplayName = "Jane Smith",
                    Id = "ef1c916a-3135-4417-ba27-8eb7bd084193",
                    AdditionalData = new Dictionary<string, object>()
                    {
                        {"userIdentityType", "aadUser"}
                    }
                }
            }
        }
    }
};

await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages
    .Request()
    .AddAsync(chatMessage);

```