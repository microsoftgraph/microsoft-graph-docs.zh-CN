---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4a729ff4c5d444c90fc21d49acb88542d080f333
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34453605"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationThread = new ConversationThread
{
    Topic = "New Conversation Thread Topic",
    Posts = new List<Post>()
    {
        new Post
        {
            Body = new ItemBody
            {
                ContentType = BodyType.Html,
                Content = "this is body content"
            },
            NewParticipants = new List<Recipient>()
            {
                new Recipient
                {
                    EmailAddress = new EmailAddress
                    {
                        Name = "Alex Darrow",
                        Address = "alexd@contoso.com"
                    }
                }
            }
        }
    }
};

await graphClient.Groups["{id}"].Threads
    .Request()
    .AddAsync(conversationThread);

```