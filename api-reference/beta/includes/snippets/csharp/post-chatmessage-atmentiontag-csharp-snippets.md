---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b574bf928a7eb8499713eb4d32afd4a1cc15b01a781fc61392ccc8abfa26041f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106934"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = new ChatMessage
{
    Body = new ItemBody
    {
        ContentType = BodyType.Html,
        Content = "<div><div><at id=\"0\">TestTag</at>&nbsp;Testing Tags</div></div>"
    },
    Mentions = new List<ChatMessageMention>()
    {
        new ChatMessageMention
        {
            Id = 0,
            MentionText = "TestTag",
            Mentioned = new ChatMessageMentionedIdentitySet
            {
                Tag = new TeamworkTagIdentity
                {
                    Id = "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM2OGEzZTM2NS1mN2Q5LTRhNTYtYjQ5OS0yNDMzMmE5Y2M1NzIjI3RTMERJZ1Z1ZQ==",
                    DisplayName = "TestTag"
                }
            }
        }
    }
};

await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages
    .Request()
    .AddAsync(chatMessage);

```