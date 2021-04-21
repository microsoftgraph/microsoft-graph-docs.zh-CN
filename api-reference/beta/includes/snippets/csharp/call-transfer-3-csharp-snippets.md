---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0972c538df699b169ff3f7e04d07d649dfbc8e69
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921007"
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