---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc48efe588b447dfee1929af5e46e13bba0970d1a256b05c9865a544125e7913
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334133"
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