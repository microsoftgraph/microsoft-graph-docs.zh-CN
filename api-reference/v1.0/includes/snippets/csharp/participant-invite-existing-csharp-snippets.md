---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c54054c16a0283d2d96277d2a86ee49e8d54dcd6
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865807"
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
    }
};

var clientContext = "f2fa86af-3c51-4bc2-8fc0-475452d9764f";

await graphClient.Communications.Calls["ab6233a5-20b7-4c5e-bea2-ce56c9776429"].Participants
    .Invite(participants,clientContext)
    .Request()
    .PostAsync();

```