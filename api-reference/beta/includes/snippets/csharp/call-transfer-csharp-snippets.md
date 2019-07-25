---
description: 自动生成的文件。 不修改
ms.openlocfilehash: de09363645eca2f6fddbb55339377c5e8459372d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708799"
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
    .Transfer(transferTarget,target,replacesCallId)
    .Request()
    .PostAsync();

```