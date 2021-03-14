---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1aada5e32f4f25f0c4fdd06a966ed7b8798826a0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789717"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversation = new Conversation
{
    Topic = "Does anyone have a second?",
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
                        Content = "This is urgent!"
                    },
                    Extensions = new PostExtensionsCollectionPage()
                    {
                        new OpenTypeExtension
                        {
                            ExtensionName = "Com.Contoso.Benefits",
                            AdditionalData = new Dictionary<string, object>()
                            {
                                {"companyName", "Contoso"},
                                {"expirationDate", "2016-08-03T11:00:00Z"},
                                {"topPicks", "[\"Employees only\",\"Add spouse or guest\",\"Add family\"]"}
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