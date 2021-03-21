---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 246e7a8907c9c945f2ec82092c44cf9dad5f61a0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957811"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var startDateTime = DateTimeOffset.Parse("2020-02-06T01:49:21.3524945+00:00");

var endDateTime = DateTimeOffset.Parse("2020-02-06T02:19:21.3524945+00:00");

var subject = "Create a meeting with customId provided";

var externalId = "7eb8263f-d0e0-4149-bb1c-1f0476083c56";

var participants = new MeetingParticipants
{
    Attendees = new List<MeetingParticipantInfo>()
    {
        new MeetingParticipantInfo
        {
            Identity = new IdentitySet
            {
                User = new Identity
                {
                    Id = "1f35f2e6-9cab-44ad-8d5a-b74c14720000"
                }
            },
            Role = OnlineMeetingRole.Presenter,
            Upn = "test1@contoso.com"
        }
    }
};

await graphClient.Me.OnlineMeetings
    .CreateOrGet(externalId,null,endDateTime,participants,startDateTime,subject)
    .Request()
    .PostAsync();

```