---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d2ec690b75b05b49a27963f5dcc068de7950bf8
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60560772"
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
    AdditionalData = new Dictionary<string, object>()
    {
        {"endpointType", "default"}
    }
};

var transferee = new ParticipantInfo
{
    Identity = new IdentitySet
    {
        User = new Identity
        {
            Id = "751f6800-3180-414d-bd94-333364659951",
            AdditionalData = new Dictionary<string, object>()
            {
                {"tenantId", "72f988bf-86f1-41af-91ab-2d7cd011db47"}
            }
        }
    },
    ParticipantId = "909c6581-5130-43e9-88f3-fcb3582cde37"
};

await graphClient.Communications.Calls["{call-id}"]
    .Transfer(transferTarget,transferee)
    .Request()
    .PostAsync();

```