---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 834fb4bdac4348c81a3a61bc4c87ee08173414ff
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302120"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var call = new Call
{
    CallbackUri = "https://bot.contoso.com/callback",
    Source = new ParticipantInfo
    {
        Identity = new IdentitySet
        {
            Application = new Identity
            {
                DisplayName = "Calling Bot",
                Id = "2891555a-92ff-42e6-80fa-6e1300c6b5c6"
            }
        },
        Region = null,
        LanguageId = null
    },
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
    MediaConfig = new AppHostedMediaConfig
    {
        Blob = "<Media Session Configuration>"
    }
};

await graphClient.Communications.Calls
    .Request()
    .AddAsync(call);

```