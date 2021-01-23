---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f1be4221834108281bdf3e46bd3f26ee23b72d91
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946290"
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

await graphClient.Groups["37df2ff0-0de0-4c33-8aee-75289364aef6"].Conversations
    .Request()
    .AddAsync(conversation);

```