---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f84e9ddd29ba565ea8399b82b178619e0e97f2f6
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865865"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var call = new Call
{
    CallbackUri = "https://bot.contoso.com/callback",
    Targets = new List<InvitationParticipantInfo>()
    {
        new InvitationParticipantInfo
        {
            Identity = new IdentitySet
            {
                User = new Identity
                {
                    DisplayName = "John",
                    Id = "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
                }
            }
        }
    },
    RequestedModalities = new List<Modality>()
    {
        Modality.Audio
    },
    MediaConfig = new ServiceHostedMediaConfig
    {
    }
};

await graphClient.Communications.Calls
    .Request()
    .AddAsync(call);

```