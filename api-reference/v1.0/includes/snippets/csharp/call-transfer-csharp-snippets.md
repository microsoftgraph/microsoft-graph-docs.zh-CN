---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc39b67da499f5d785ffd405f778b1bb69101b85
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865832"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var transferTarget = new InvitationParticipantInfo
{
    EndpointType = "default",
    Identity = new IdentitySet
    {
        User = new Identity
        {
            Id = "550fae72-d251-43ec-868c-373732c2704f",
            DisplayName = "Heidi Steen"
        }
    },
    ReplacesCallId = "replacesCallId-value"
};

var clientContext = "9e90d1c1-f61e-43e7-9f75-d420159aae08";

await graphClient.Communications.Calls["{id}"]
    .Transfer(transferTarget)
    .Request()
    .PostAsync();

```