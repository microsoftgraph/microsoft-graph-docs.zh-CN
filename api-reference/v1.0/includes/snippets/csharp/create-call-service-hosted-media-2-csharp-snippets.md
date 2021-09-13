---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 38de12e28cbc6691875e26710de7c8e1b6e9005aec448298d750483f79c61529
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278723"
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
            AdditionalData = new Dictionary<string, object>()
            {
                {"applicationInstance", "{\"@odata.type\":\"#microsoft.graph.identity\",\"displayName\":\"Calling Bot\",\"id\":\"3d913abb-aec0-4964-8fa6-3c6850c4f278\"}"}
            }
        },
        CountryCode = null,
        EndpointType = null,
        Region = null,
        LanguageId = null
    },
    Targets = new List<InvitationParticipantInfo>()
    {
        new InvitationParticipantInfo
        {
            Identity = new IdentitySet
            {
                AdditionalData = new Dictionary<string, object>()
                {
                    {"phone", "{\"@odata.type\":\"#microsoft.graph.identity\",\"id\":\"+12345678901\"}"}
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
    },
    TenantId = "aa67bd4c-8475-432d-bd41-39f255720e0a"
};

await graphClient.Communications.Calls
    .Request()
    .AddAsync(call);

```