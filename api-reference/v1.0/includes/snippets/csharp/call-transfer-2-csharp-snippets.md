---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 63f5ca18fe422e7267a9a51415831b1f68f414b2
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/06/2021
ms.locfileid: "60217826"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var transferTarget = new InvitationParticipantInfo
{
    Identity = new IdentitySet
    {
        User = new Identity
        {
            Id = "550fae72-d251-43ec-868c-373732c2704f",
            DisplayName = "Heidi Steen"
        }
    },
    ReplacesCallId = "e5d39592-99bd-4db8-bca8-30fb894ec51d",
    AdditionalData = new Dictionary<string, object>()
    {
        {"endpointType", "default"}
    }
};

await graphClient.Communications.Calls["{call-id}"]
    .Transfer(transferTarget,null)
    .Request()
    .PostAsync();

```