---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4634e6190967850d5cc9827cf10bccc5c70265e4
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093661"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var siteSource = new Microsoft.Graph.Ediscovery.SiteSource
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"site@odata.bind", "https://graph.microsoft.com/v1.0/sites/{siteId}"}
    }
};

await graphClient.Compliance.Ediscovery.Cases["4c8f8f70-7785-4bd4-b296-c98376a2c5e1"].Custodians["2192ca408ea2410eba3bec8ae873be6b"].SiteSources
    .Request()
    .AddAsync(siteSource);

```