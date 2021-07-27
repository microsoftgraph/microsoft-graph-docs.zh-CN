---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 149ce4a0d95bb518ceabc27c38bb17c3c1bf4af1
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53579531"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = new ChatMessage
{
    Body = new ItemBody
    {
        ContentType = BodyType.Html,
        Content = "<div><div><at id=\"0\">General</at>&nbsp;Hello there!</div></div>"
    },
    Mentions = new List<ChatMessageMention>()
    {
        new ChatMessageMention
        {
            Id = 0,
            MentionText = "General",
            Mentioned = new ChatMessageMentionedIdentitySet
            {
                Conversation = new TeamworkConversationIdentity
                {
                    Id = "19:0b50940236084d258c97b21bd01917b0@thread.skype",
                    DisplayName = "General",
                    ConversationIdentityType = TeamworkConversationIdentityType.Channel
                }
            }
        }
    }
};

await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages
    .Request()
    .AddAsync(chatMessage);

```