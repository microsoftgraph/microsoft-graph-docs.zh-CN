---
description: 自动生成的文件。 不修改
ms.openlocfilehash: da8c04b64f26d5029e08232f8baed651120a6687
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878353"
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
                            AdditionalData = new Dictionary<string, object>()
                            {
                                {"@odata.type","microsoft.graph.openTypeExtension"}
                            },
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