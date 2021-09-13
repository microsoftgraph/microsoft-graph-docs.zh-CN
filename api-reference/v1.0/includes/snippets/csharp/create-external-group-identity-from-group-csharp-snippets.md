---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f757cf3225671a36e4d09e926d070410e94172d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59022630"
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