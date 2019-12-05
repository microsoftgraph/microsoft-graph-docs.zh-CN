---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6dd0a007134c5c27e315beebdce6537bb07491a0
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2019
ms.locfileid: "39856730"
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
    MediaConfig = new AppHostedMediaConfig
    {
        Blob = "<Media Session Configuration>"
    }
};

await graphClient.Communications.Calls
    .Request()
    .AddAsync(call);

```