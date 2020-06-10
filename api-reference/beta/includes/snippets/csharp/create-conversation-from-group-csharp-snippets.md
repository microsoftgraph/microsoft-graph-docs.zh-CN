---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46b83c54e9201267d10ca9d37a00685326ce774f
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44685176"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversation = new Conversation
{
    Topic = "New head count",
    Threads = (IConversationThreadsCollectionPage)new List<ConversationThread>()
    {
        new ConversationThread
        {
            Posts = (IConversationThreadPostsCollectionPage)new List<Post>()
            {
                new Post
                {
                    Body = new ItemBody
                    {
                        ContentType = BodyType.Html,
                        Content = "The confirmation will come by the end of the week."
                    },
                    NewParticipants = new List<Recipient>()
                    {
                        new Recipient
                        {
                            EmailAddress = new EmailAddress
                            {
                                Name = "Adele Vance",
                                Address = "AdeleV@contoso.onmicrosoft.com"
                            }
                        }
                    }
                }
            }
        }
    }
};

await graphClient.Groups["29981b6a-0e57-42dc-94c9-cd24f5306196"].Conversations
    .Request()
    .AddAsync(conversation);

```