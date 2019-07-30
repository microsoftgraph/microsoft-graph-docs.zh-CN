---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ef1702cdb00e0c5920049b789a7fcdece1d20573
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933811"
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
            TenantId = "72f988bf-86f1-41af-91ab-2d7cd011db47",
            DisplayName = "Heidi Steen"
        }
    },
    LanguageId = "languageId-value",
    Region = "region-value",
    ReplacesCallId = "replacesCallId-value"
};

var clientContext = "clientContext-value";

await graphClient.App.Calls["{id}"]
    .Transfer(transferTarget)
    .Request()
    .PostAsync();

```