---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e1d5090eb0c15c455a8f48ea9eed2d9a103847f
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093615"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var custodian = new Microsoft.Graph.Ediscovery.Custodian
{
    Email = "AdeleV@contoso.com",
    ApplyHoldToSources = true
};

await graphClient.Compliance.Ediscovery.Cases["2192ca408ea2410eba3bec8ae873be6b"].Custodians
    .Request()
    .AddAsync(custodian);

```