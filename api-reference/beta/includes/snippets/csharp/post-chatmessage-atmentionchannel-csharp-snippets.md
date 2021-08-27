---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0718863acd6784ad5fcbb77f04153f0cdc354ccfe00fbfe3a4fe0566dc7b25d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106937"
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