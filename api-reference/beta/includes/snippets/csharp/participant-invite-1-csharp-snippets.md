---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 386ca786ceee53c18c75f1a51d15dda1448852b216d2bb2fcfc9037589f0c98f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161675"
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

await graphClient.Communications.Calls["{call-id}"].Participants
    .Invite(participants,clientContext)
    .Request()
    .PostAsync();

```