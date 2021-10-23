---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b8e9ac32aa90da3b5fc0c0e5811e04ca76b4f33
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561020"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var meetingRegistration = new MeetingRegistration
{
    Subject = "Microsoft Ignite: Day 1",
    StartDateTime = DateTimeOffset.Parse("2021-11-02T16:00:00+00:00"),
    EndDateTime = DateTimeOffset.Parse("2021-11-02T23:45:00+00:00"),
    Speakers = new List<MeetingSpeaker>()
    {
        new MeetingSpeaker
        {
            DisplayName = "Henry Ross",
            Bio = "Chairman and Chief Executive Officer"
        },
        new MeetingSpeaker
        {
            DisplayName = "Fred Ryan",
            Bio = "CVP"
        }
    }
};

await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"].Registration
    .Request()
    .UpdateAsync(meetingRegistration);

```