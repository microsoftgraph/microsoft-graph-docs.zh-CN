---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46ab0f0e5bf1d74fa47320049766b62f050eab9a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773233"
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

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Custodians["{ediscovery.custodian-id}"].UnifiedGroupSources
    .Request()
    .AddAsync(unifiedGroupSource);

```