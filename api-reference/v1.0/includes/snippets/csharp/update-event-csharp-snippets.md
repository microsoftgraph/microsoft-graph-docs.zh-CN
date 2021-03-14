---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e689482f00423c6ff1c7a643a6991e8c7556609a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803498"
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
        Time = DateTimeOffset.Parse("datetime-value")
    },
    Recurrence = null,
    ICalUId = "iCalUId-value",
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