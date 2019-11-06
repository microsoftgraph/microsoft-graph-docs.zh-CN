---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37c238052f20e46d82ecb4248936d44822b7377b
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "38000172"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var call = new Call
{
    CallbackUri = "https://bot.contoso.com/callback",
    Targets = new List<InvitationParticipantInfo>()
    {
        new ParticipantInfo
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

await graphClient.App.Calls
    .Request()
    .Header("Authorization","Bearer <Token>")
    .AddAsync(call);

```