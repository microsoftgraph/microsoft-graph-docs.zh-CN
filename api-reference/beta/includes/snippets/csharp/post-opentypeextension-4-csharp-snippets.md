---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7e23bf3d888dfce1a89130c1f7a05e70c5bdde1d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878356"
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
            AdditionalData = new Dictionary<string, object>()
            {
                {"@odata.type","microsoft.graph.openTypeExtension"}
            },
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