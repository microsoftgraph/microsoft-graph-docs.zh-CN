---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d177f50b61272136cdbec063e9ada238e3cb6e9b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779788"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversation = new Conversation
{
    Topic = "New head count",
    Threads = new ConversationThreadsCollectionPage()
    {
        new ConversationThread
        {
            Posts = new ConversationThreadPostsCollectionPage()
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

await graphClient.Groups["{group-id}"].Conversations
    .Request()
    .AddAsync(conversation);

```