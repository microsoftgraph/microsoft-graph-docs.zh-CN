---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6096954d41ba704a8a1a7dfe5ab49406d326931b
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470873"
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

await graphClient.Groups["37df2ff0-0de0-4c33-8aee-75289364aef6"].Threads["AAQkADJizZJpEWwqDHsEpV_KA=="].Posts["AAMkADJiUg96QZUkA-ICwMubAAC1heiSAAA="]
    .Reply(post)
    .Request()
    .PostAsync();

```