---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c470b357768c6b97497704e9bd5e997325511ba
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945106"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationThread = new ConversationThread
{
    Topic = "New Conversation Thread Topic",
    Posts = new ConversationThreadPostsCollectionPage()
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