---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3fb3710806a85def726dc2b24b6adc7620a108c6
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472276"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var call = new Call
{
    CallbackUri = "https://bot.contoso.com/callback",
    RequestedModalities = new List<Modality>()
    {
        Modality.Audio
    },
    MediaConfig = new ServiceHostedMediaConfig
    {
        PreFetchMedia = new List<MediaInfo>()
        {
            new MediaInfo
            {
                Uri = "https://cdn.contoso.com/beep.wav",
                ResourceId = "f8971b04-b53e-418c-9222-c82ce681a582"
            },
            new MediaInfo
            {
                Uri = "https://cdn.contoso.com/cool.wav",
                ResourceId = "86dc814b-c172-4428-9112-60f8ecae1edb"
            }
        }
    },
    ChatInfo = new ChatInfo
    {
        ThreadId = "19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2",
        MessageId = "0"
    },
    MeetingInfo = new OrganizerMeetingInfo
    {
        Organizer = new IdentitySet
        {
            User = new Identity
            {
                Id = "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
                DisplayName = "Bob",
                AdditionalData = new Dictionary<string, object>()
                {
                    {"tenantId", "86dc81db-c112-4228-9222-63f3esaa1edb"}
                }
            }
        },
        AllowConversationWithoutHost = true
    },
    TenantId = "86dc81db-c112-4228-9222-63f3esaa1edb"
};

await graphClient.Communications.Calls
    .Request()
    .AddAsync(call);

```