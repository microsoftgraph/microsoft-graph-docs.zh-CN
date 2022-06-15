---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b337796543bae25050f74e6004474490c11a9b17
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093491"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ediscoveryCustodian = new Microsoft.Graph.Security.EdiscoveryCustodian
{
    Email = "AdeleV@contoso.com"
};

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Custodians
    .Request()
    .AddAsync(ediscoveryCustodian);

```