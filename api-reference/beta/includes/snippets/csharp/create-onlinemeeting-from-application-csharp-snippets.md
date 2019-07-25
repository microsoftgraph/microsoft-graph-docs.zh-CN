---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 76da270d9670b6e83a4192f8eda741b0f2306f3b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711471"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var OnlineMeeting = new OnlineMeeting
{
    MeetingType = MeetingType.MeetNow,
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
    },
    Subject = "subject-value"
};

await graphClient.App.OnlineMeetings
    .Request()
    .AddAsync(OnlineMeeting);

```