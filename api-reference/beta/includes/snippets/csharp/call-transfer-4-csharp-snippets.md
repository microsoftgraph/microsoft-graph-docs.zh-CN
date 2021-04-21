---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 66baf3a4b265af1102cc972dc33e7e9dbb2a304d
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921015"
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
    .Transfer(transferTarget)
    .Request()
    .PostAsync();

```