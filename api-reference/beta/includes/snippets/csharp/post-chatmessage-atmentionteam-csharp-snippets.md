---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00943036302381e6de722d07705414b1f7e72d36
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53579538"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = new ChatMessage
{
    Body = new ItemBody
    {
        ContentType = BodyType.Html,
        Content = "<div><div><at id=\"0\">GraphTesting</at>&nbsp;Hello team</div></div>"
    },
    Mentions = new List<ChatMessageMention>()
    {
        new ChatMessageMention
        {
            Id = 0,
            MentionText = "GraphTesting",
            Mentioned = new ChatMessageMentionedIdentitySet
            {
                Conversation = new TeamworkConversationIdentity
                {
                    Id = "68a3e365-f7d9-4a56-b499-24332a9cc572",
                    DisplayName = "GraphTesting",
                    ConversationIdentityType = TeamworkConversationIdentityType.Team
                }
            }
        }
    },
    Reactions = new List<ChatMessageReaction>()
    {
    }
};

await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages
    .Request()
    .AddAsync(chatMessage);

```