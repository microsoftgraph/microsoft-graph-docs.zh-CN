---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33824977d12bb774a882df18cdfecdf67edabd58
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65316253"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var participants = new List<InvitationParticipantInfo>()
{
    new InvitationParticipantInfo
    {
        ReplacesCallId = "a7ebfb2d-871e-419c-87af-27290b22e8db",
        ParticipantId = "7d501bf1-5ee4-4605-ba92-0ae4513c611c",
        Identity = new IdentitySet
        {
            User = new Identity
            {
                Id = "682b6c37-0729-4fab-ace6-d730d5d9137e",
                AdditionalData = new Dictionary<string, object>()
                {
                    {"identityProvider", "AAD"}
                }
            }
        }
    }
};

var clientContext = "f2fa86af-3c51-4bc2-8fc0-475452d9764f";

await graphClient.Communications.Calls["{call-id}"].Participants
    .Invite(participants,clientContext)
    .Request()
    .PostAsync();

```