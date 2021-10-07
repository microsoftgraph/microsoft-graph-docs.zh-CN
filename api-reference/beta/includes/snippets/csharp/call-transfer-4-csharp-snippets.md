---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1de1568891d7faf62b56b0132b6a93cd26d4e52b
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214521"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var transferTarget = new InvitationParticipantInfo
{
    EndpointType = EndpointType.Default,
    Identity = new IdentitySet
    {
        AdditionalData = new Dictionary<string, object>()
        {
            {"phone", "{\"@odata.type\":\"#microsoft.graph.identity\",\"id\":\"+12345678901\"}"}
        }
    },
    ReplacesCallId = "e5d39592-99bd-4db8-bca8-30fb894ec51d",
    AdditionalData = new Dictionary<string, object>()
    {
        {"languageId", "en-us"},
        {"region", "amer"}
    }
};

await graphClient.Communications.Calls["{call-id}"]
    .Transfer(transferTarget,null)
    .Request()
    .PostAsync();

```