---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e0588b3a3d39027edd12556ad1f780639c256ba
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093685"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userSource = new Microsoft.Graph.Ediscovery.UserSource
{
    Email = "megan@contoso.com",
    IncludedSources = Microsoft.Graph.Ediscovery.SourceType.Mailbox | Microsoft.Graph.Ediscovery.SourceType.Site
};

await graphClient.Compliance.Ediscovery.Cases["4c8f8f70-7785-4bd4-b296-c98376a2c5e1"].Custodians["2192ca408ea2410eba3bec8ae873be6b"].UserSources
    .Request()
    .AddAsync(userSource);

```