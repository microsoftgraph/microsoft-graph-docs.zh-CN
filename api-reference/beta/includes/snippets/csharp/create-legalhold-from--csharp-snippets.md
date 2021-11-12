---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 947c3ab4addfa6c742c205acee91ea0daa9c02924e671b4dad191a1a4980b6ae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378286"
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