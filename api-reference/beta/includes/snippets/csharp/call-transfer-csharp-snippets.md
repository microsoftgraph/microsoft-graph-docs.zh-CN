---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39c2f07f628dabaf34b2cddae56dff5ea6588cb2
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302736"
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

var clientContext = "9e90d1c1-f61e-43e7-9f75-d420159aae08";

await graphClient.Communications.Calls["{id}"]
    .Transfer(transferTarget)
    .Request()
    .PostAsync();

```