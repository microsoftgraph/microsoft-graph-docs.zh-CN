---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 48318049b5102ed019f262ce741c2c6cbb7306cb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779545"
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
                Id = "7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
                DisplayName = "string"
            }
        }
    },
    new InvitationParticipantInfo
    {
        ReplacesCallId = "a7ebfb2d-871e-419c-87af-27290b22e8db",
        Identity = new IdentitySet
        {
            User = new Identity
            {
                Id = "1e126418-44a0-4a94-a6f8-0efe1ad71acb",
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