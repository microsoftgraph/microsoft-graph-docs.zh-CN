---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a528eaa203db4787c9d55db2bbdbb4113b466e36
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942669"
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
    }
};

await graphClient.Communications.Calls
    .Request()
    .AddAsync(call);

```