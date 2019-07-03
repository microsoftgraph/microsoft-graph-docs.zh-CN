---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bf0ac7a9f04202b3ed20b5169f2b385028984aa6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500196"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extension = new Extension
{
    ExtensionName = "Com.Contoso.Estimate",
    CompanyName = "Contoso",
    ExpirationDate = "2016-07-30T11:00:00Z",
    DealValue = 1010100,
    TopPicks = new List<String>()
    {
        "Employees only",
        "Add spouse or guest",
        "Add family"
    }
};

await graphClient.Groups["37df2ff0-0de0-4c33-8aee-75289364aef6"].Threads["AAQkADJizZJpEWwqDHsEpV_KA=="].Posts["AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA="].Extensions["Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate"]
    .Request()
    .UpdateAsync(extension);

```