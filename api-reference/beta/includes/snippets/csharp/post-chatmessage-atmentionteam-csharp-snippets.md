---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c93e1b565e65cca353687a54432cba6f7b1fe4c6692dffa1d760dd08e930e2e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106933"
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