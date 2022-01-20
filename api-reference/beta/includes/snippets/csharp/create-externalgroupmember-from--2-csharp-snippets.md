---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3292abef821790ffe4d0526f04780e678bb3ffc0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137666"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identity = new Microsoft.Graph.ExternalConnectors.Identity
{
    Id = "e5477431-1038-484e-bf69-1dfedb97a110",
    Type = Microsoft.Graph.ExternalConnectors.IdentityType.ExternalGroup
};

await graphClient.External.Connections["{externalConnectors.externalConnection-id}"].Groups["{externalConnectors.externalGroup-id}"].Members
    .Request()
    .AddAsync(identity);

```