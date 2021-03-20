---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 536275243f953215fe91c7a3f33e23e1ce4be41b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945148"
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
                DisplayName = "string"
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