---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3097f8020c2f4c8655ef958c1ba4938db8346692547673f09125f697bb483e07
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221370"
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