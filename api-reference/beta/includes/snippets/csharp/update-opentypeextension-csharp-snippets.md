---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d3c088133c5f37bbcca4ad84edace1d4330a734b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878144"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extension = new Extension
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.type","#microsoft.outlookServices.openTypeExtension"}
    },
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