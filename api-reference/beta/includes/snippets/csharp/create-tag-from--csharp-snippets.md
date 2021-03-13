---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 858bc389854c8891b69031160b9d4da6248434b6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773779"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tag = new Microsoft.Graph.Ediscovery.Tag
{
    DisplayName = "Privileged",
    Description = "The document is privileged",
    AdditionalData = new Dictionary<string, object>()
    {
        {"parent@odata.bind", "https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/98fdad78bbce4519b75474bc150575c3"}
    }
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Tags
    .Request()
    .AddAsync(tag);

```