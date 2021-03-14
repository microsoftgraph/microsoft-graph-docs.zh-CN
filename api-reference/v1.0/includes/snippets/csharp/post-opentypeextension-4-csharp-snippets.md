---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06247bf5f22eb3606d8e3427ac7e940e148846f8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792041"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var post = new Post
{
    Body = new ItemBody
    {
        ContentType = BodyType.Html,
        Content = "<html><body><div><div><div><div>When and where? </div></div></div></div></body></html>"
    },
    Extensions = new PostExtensionsCollectionPage()
    {
        new OpenTypeExtension
        {
            ExtensionName = "Com.Contoso.HR",
            AdditionalData = new Dictionary<string, object>()
            {
                {"companyName", "Contoso"},
                {"expirationDate", "2015-07-03T13:04:00Z"},
                {"topPicks", "[\"Employees only\",\"Add spouse or guest\",\"Add family\"]"}
            }
        }
    }
};

await graphClient.Groups["{group-id}"].Threads["{conversationThread-id}"].Posts["{post-id}"]
    .Reply(post)
    .Request()
    .PostAsync();

```