---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 47e47169e3d2869da28ad03411db684a090b6c4f
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933791"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onlineMeeting = new OnlineMeeting
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
    .AddAsync(onlineMeeting);

```