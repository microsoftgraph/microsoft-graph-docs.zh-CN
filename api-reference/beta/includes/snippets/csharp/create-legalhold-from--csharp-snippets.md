---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa0a489324f883061a461e8df82d763fab02ca86
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2021
ms.locfileid: "51987545"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var legalHold = new Microsoft.Graph.Ediscovery.LegalHold
{
    Description = "String",
    CreatedBy = new IdentitySet
    {
    },
    IsEnabled = false,
    Status = Microsoft.Graph.Ediscovery.LegalHoldStatus.Pending,
    ContentQuery = "String",
    Errors = new List<String>()
    {
        "String"
    },
    DisplayName = "String"
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].LegalHolds
    .Request()
    .AddAsync(legalHold);

```