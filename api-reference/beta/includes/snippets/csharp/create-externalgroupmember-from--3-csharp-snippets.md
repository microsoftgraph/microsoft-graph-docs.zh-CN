---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f757cf3225671a36e4d09e926d070410e94172d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137664"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identity = new Microsoft.Graph.ExternalConnectors.Identity
{
    Id = "1431b9c38ee647f6a",
    Type = Microsoft.Graph.ExternalConnectors.IdentityType.ExternalGroup
};

await graphClient.External.Connections["{externalConnectors.externalConnection-id}"].Groups["{externalConnectors.externalGroup-id}"].Members
    .Request()
    .AddAsync(identity);

```