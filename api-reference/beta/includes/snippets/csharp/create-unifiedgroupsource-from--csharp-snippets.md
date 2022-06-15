---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ede3b77d5505aa58bee9abad535188ab170cee4
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092819"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedGroupSource = new Microsoft.Graph.Security.UnifiedGroupSource
{
    IncludedSources = Microsoft.Graph.Security.SourceType.Mailbox,
    AdditionalData = new Dictionary<string, object>()
    {
        {"group@odata.bind", "https://graph.microsoft.com/v1.0/groups/93f90172-fe05-43ea-83cf-ff785a40d610"}
    }
};

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Custodians["{security.ediscoveryCustodian-id}"].UnifiedGroupSources
    .Request()
    .AddAsync(unifiedGroupSource);

```