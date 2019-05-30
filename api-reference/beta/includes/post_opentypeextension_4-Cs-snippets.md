---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ffb6156f30b6d3074fa20d285d6c6e9f3425c34f
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34546607"
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
    Extensions = new List<Extension>()
    {
        new Extension
        {
            ExtensionName = "Com.Contoso.HR",
            CompanyName = "Contoso",
            ExpirationDate = "2015-07-03T13:04:00Z",
            TopPicks = new List<String>()
            {
                "Employees only",
                "Add spouse or guest",
                "Add family"
            }
        }
    }
};

await graphClient.Groups["37df2ff0-0de0-4c33-8aee-75289364aef6"].Threads["AAQkADJizZJpEWwqDHsEpV_KA=="].Posts["AAMkADJiUg96QZUkA-ICwMubAAC1heiSAAA="]
    .Reply(post)
    .Request()
    .PostAsync();

```