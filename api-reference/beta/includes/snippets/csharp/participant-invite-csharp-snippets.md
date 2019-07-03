---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c1aec6d469d0ab2d16317ade124d9c9bb20b8cbe
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500683"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var participants = new List<InvitationParticipantInfo>()
{
    new InvitationParticipantInfo
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
    }
};

var clientContext = "clientContext-value";

await graphClient.App.Calls["{id}"].Participants
    .Invite(participants,clientContext)
    .Request()
    .PostAsync();

```