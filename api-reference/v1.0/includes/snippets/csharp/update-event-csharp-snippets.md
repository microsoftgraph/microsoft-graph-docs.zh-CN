---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49ff221b209033a89f58a47a449892df9bad98526bf4db91c9537408118adadd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332339"
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