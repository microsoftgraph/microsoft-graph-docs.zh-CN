---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eae53cc58a6a30b86bdb92c8f35640baf5040b8d
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428788"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onlineMeeting = new OnlineMeeting
{
    MeetingType = "meetNow",
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
    .AddAsync(onlineMeeting);

```