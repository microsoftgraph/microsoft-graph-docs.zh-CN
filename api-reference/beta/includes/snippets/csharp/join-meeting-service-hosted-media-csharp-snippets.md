---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf86b1ec8a023a5853a2bf2e07682e4969ff93bd
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60983135"
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
                    {"tenantId", "9f386a15-f9cc-445b-8106-ac85e314a07b"}
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