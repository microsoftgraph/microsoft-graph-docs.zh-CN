---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71651cb9ec02dfe1e96d4e9fbe1ad15e6b5b8447
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684052"
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

await graphClient.Groups["37df2ff0-0de0-4c33-8aee-75289364aef6"].Threads["AAQkADJizZJpEWwqDHsEpV_KA=="].Posts["AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA="].Extensions["Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate"]
    .Request()
    .UpdateAsync(extension);

```