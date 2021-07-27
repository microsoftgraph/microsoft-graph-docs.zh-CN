---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49ca20431b2a5a79da402be8bfdadb6fb981ccb8
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53579534"
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