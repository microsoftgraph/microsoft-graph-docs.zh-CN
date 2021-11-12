---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 08d6fb6f34339353bdcbcce0dc5a222cfbf7d88ae858542335846126629ecf9f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219554"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var custodian = new Microsoft.Graph.Ediscovery.Custodian
{
    Email = "AdeleV@contoso.com",
    ApplyHoldToSources = true
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Custodians
    .Request()
    .AddAsync(custodian);

```