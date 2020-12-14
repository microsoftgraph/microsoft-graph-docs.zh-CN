---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c59d0e671ae5a892d0b241adc65cabdf677c514
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659050"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedGroupSource = new UnifiedGroupSource
{
    IncludedSources = SourceType.Mailbox | SourceType.Site,
    AdditionalData = new Dictionary<string, object>()
    {
        {"group@odata.bind", "/groups/000044f9-47c8-4a87-bccf-291fbf006a54"}
    }
};

await graphClient.Compliance.Ediscovery.Cases["{ediscoveryCaseId}"].Custodians["{custodianId}"].UnifiedGroupSources
    .Request()
    .AddAsync(unifiedGroupSource);

```