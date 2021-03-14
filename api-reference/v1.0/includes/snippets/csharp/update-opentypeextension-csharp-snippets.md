---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49b5df978c36123e6ebf64871d65cfe9b342a60d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792498"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extension = new OpenTypeExtension
{
    ExtensionName = "Com.Contoso.Estimate",
    AdditionalData = new Dictionary<string, object>()
    {
        {"companyName", "Contoso"},
        {"expirationDate", "2016-07-30T11:00:00Z"},
        {"DealValue", "1010100"},
        {"topPicks", "[\"Employees only\",\"Add spouse or guest\",\"Add family\"]"}
    }
};

await graphClient.Groups["{group-id}"].Threads["{conversationThread-id}"].Posts["{post-id}"].Extensions["{extension-id}"]
    .Request()
    .UpdateAsync(extension);

```