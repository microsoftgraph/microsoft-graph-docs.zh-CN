---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2ae8025b1c98f16090af1c60ec1a63e7288fc2c
ms.sourcegitcommit: c75356177c73ec480cec868a4404a63dca5b078d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2020
ms.locfileid: "43512313"
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
    OnlineMeetingProvider = "teamsForBusiness",
    IsReminderOn = true
};

await graphClient.Me.Events["{id}"]
    .Request()
    .UpdateAsync(@event);

```