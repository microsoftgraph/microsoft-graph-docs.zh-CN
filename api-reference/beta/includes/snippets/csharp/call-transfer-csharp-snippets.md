---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0972c538df699b169ff3f7e04d07d649dfbc8e69
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573151"
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
    AdditionalData = new Dictionary<string, object>()
    {
        {"languageId", "languageId-value"},
        {"region", "region-value"}
    }
};

await graphClient.Communications.Calls["{call-id}"]
    .Transfer(transferTarget)
    .Request()
    .PostAsync();

```