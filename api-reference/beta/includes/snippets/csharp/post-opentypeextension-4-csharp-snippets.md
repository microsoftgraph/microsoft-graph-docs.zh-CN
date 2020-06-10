---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 98e26ef3132ad118c49e79b0e47e1d1456d285d0
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683732"
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
    Extensions = (IPostExtensionsCollectionPage)new List<Extension>()
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

await graphClient.Groups["37df2ff0-0de0-4c33-8aee-75289364aef6"].Threads["AAQkADJizZJpEWwqDHsEpV_KA=="].Posts["AAMkADJiUg96QZUkA-ICwMubAAC1heiSAAA="]
    .Reply(post)
    .Request()
    .PostAsync();

```