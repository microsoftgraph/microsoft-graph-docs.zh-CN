---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71fc8b7df3c40658382017e3bc3affeaec265513
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093672"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var custodian = new Microsoft.Graph.Ediscovery.Custodian
{
    ApplyHoldToSources = false
};

await graphClient.Compliance.Ediscovery.Cases["2192ca408ea2410eba3bec8ae873be6b"].Custodians["45454331323337443946343043464239"]
    .Request()
    .UpdateAsync(custodian);

```