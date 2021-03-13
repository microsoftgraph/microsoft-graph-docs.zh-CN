---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3bb7c2e8bda2a5df6f25ba1f217ec1b19813032f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796240"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = new Event
{
    OriginalStartTimeZone = "originalStartTimeZone-value",
    OriginalEndTimeZone = "originalEndTimeZone-value",
    ResponseStatus = new ResponseStatus
    {
        Response = ResponseType.None,
        Time = DateTimeOffset.Parse("2016-10-19T10:37:00Z")
    },
    Recurrence = null,
    Uid = "iCalUId-value",
    ReminderMinutesBeforeStart = 99,
    IsOnlineMeeting = true,
    OnlineMeetingProvider = OnlineMeetingProviderType.TeamsForBusiness,
    IsReminderOn = true,
    HideAttendees = false,
    Categories = new List<String>()
    {
        "Red category"
    }
};

await graphClient.Me.Events["{event-id}"]
    .Request()
    .UpdateAsync(@event);

```