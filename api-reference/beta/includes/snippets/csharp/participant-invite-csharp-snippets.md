---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd04de98637b96c9bc4e5c244aed3a0a71d77db6
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683664"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var participants = new List<InvitationParticipantInfo>()
{
    new InvitationParticipantInfo
    {
        ReplacesCallId = "a7ebfb2d-871e-419c-87af-27290b22e8db",
        Identity = new IdentitySet
        {
            User = new Identity
            {
                Id = "278405a3-f568-4b3e-b684-009193463064",
                AdditionalData = new Dictionary<string, object>()
                {
                    {"identityProvider", "AAD"}
                }
            }
        }
    }
};

var clientContext = "f2fa86af-3c51-4bc2-8fc0-475452d9764f";

await graphClient.Communications.Calls["{id}"].Participants
    .Invite(participants,clientContext)
    .Request()
    .PostAsync();

```