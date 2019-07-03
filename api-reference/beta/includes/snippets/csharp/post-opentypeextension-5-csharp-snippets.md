---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f94b31191afecde70b503c1622cfea74a22e1fc2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478985"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversation = new Conversation
{
    Topic = "Does anyone have a second?",
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
                        Content = "This is urgent!"
                    },
                    Extensions = new List<Extension>()
                    {
                        new Extension
                        {
                            ExtensionName = "Com.Contoso.Benefits",
                            CompanyName = "Contoso",
                            ExpirationDate = "2016-08-03T11:00:00Z",
                            TopPicks = new List<String>()
                            {
                                "Employees only",
                                "Add spouse or guest",
                                "Add family"
                            }
                        }
                    }
                }
            }
        }
    }
};

await graphClient.Groups["37df2ff0-0de0-4c33-8aee-75289364aef6"].Conversations
    .Request()
    .AddAsync(conversation);

```