---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 70f85f8e72de6004fb7daa32d65ae69d1706d1c35ca646199b7b2005de9a883b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221371"
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