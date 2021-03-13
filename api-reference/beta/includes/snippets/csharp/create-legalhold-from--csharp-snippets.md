---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c4a64d2945a0e7852d7b90694ac361a608370ac9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773842"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var legalHold = new LegalHold
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