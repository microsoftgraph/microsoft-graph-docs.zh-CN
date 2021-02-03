---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc02a14d4bacdd389ba41ceafe766ddb21f4d029
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093675"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedGroupSource = new Microsoft.Graph.Ediscovery.UnifiedGroupSource
{
    IncludedSources = Microsoft.Graph.Ediscovery.SourceType.Mailbox | Microsoft.Graph.Ediscovery.SourceType.Site,
    AdditionalData = new Dictionary<string, object>()
    {
        {"group@odata.bind", "/groups/000044f9-47c8-4a87-bccf-291fbf006a54"}
    }
};

await graphClient.Compliance.Ediscovery.Cases["{ediscoveryCaseId}"].Custodians["{custodianId}"].UnifiedGroupSources
    .Request()
    .AddAsync(unifiedGroupSource);

```