---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c988b4a959e4e5889f8cdaae64782ea575120204
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 09/16/2020
ms.locfileid: "47842790"
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
            Upn = "test1@contoso.com"
        }
    }
};

await graphClient.Me.OnlineMeetings
    .CreateOrGet(externalId,null,endDateTime,participants,startDateTime,subject)
    .Request()
    .PostAsync();

```