---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bf0ac7a9f04202b3ed20b5169f2b385028984aa6
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34546646"
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