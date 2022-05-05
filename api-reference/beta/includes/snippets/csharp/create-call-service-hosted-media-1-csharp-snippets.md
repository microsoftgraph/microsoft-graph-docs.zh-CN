---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4549b65d4af79ab2712be0f699c7e9ca5660a43c
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220263"
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
    CallOptions = new OutgoingCallOptions
    {
        IsContentSharingNotificationEnabled = true
    },
    MediaConfig = new ServiceHostedMediaConfig
    {
    }
};

await graphClient.Communications.Calls
    .Request()
    .AddAsync(call);

```