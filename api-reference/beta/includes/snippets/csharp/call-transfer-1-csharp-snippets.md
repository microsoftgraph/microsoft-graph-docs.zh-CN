---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 929e2830a0e65c22d979ce2cac20f025969cea56
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214522"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var transferTarget = new InvitationParticipantInfo
{
    EndpointType = EndpointType.Default,
    Identity = new IdentitySet
    {
        User = new Identity
        {
            Id = "550fae72-d251-43ec-868c-373732c2704f",
            DisplayName = "Heidi Steen",
            AdditionalData = new Dictionary<string, object>()
            {
                {"tenantId", "72f988bf-86f1-41af-91ab-2d7cd011db47"}
            }
        }
    },
    AdditionalData = new Dictionary<string, object>()
    {
        {"languageId", "languageId-value"},
        {"region", "region-value"}
    }
};

await graphClient.Communications.Calls["{call-id}"]
    .Transfer(transferTarget,null)
    .Request()
    .PostAsync();

```