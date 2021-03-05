---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71651cb9ec02dfe1e96d4e9fbe1ad15e6b5b8447
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470715"
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