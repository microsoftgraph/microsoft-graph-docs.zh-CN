---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d9421c7191a2b98005cb828eac8155ac6a03460
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40911882"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onlineMeeting = new OnlineMeeting
{
    StartDateTime = DateTimeOffset.Parse("2019-09-09T21:33:30.8546353+00:00"),
    EndDateTime = DateTimeOffset.Parse("2019-09-09T22:03:30.8566356+00:00"),
    Subject = "Application Token Meeting",
    Participants = new MeetingParticipants
    {
        Organizer = new MeetingParticipantInfo
        {
            Identity = new IdentitySet
            {
                User = new Identity
                {
                    Id = "550fae72-d251-43ec-868c-373732c2704f"
                }
            }
        }
    }
};

await graphClient.Communications.OnlineMeetings
    .Request()
    .AddAsync(onlineMeeting);

```