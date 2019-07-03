---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 13ecb4ff895ffbef10fd715b269b4437a5ff7450
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509332"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversation = new Conversation
{
    Topic = "New locations for this quarter",
    Threads = new List<ConversationThread>()
    {
        new ConversationThread
        {
            Posts = new List<Post>()
            {
                new Post
                {
                    Body = new ItemBody
                    {
                        ContentType = BodyType.Html,
                        Content = "What do we know so far?"
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