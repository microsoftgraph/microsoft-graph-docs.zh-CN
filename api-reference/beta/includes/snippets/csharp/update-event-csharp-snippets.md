---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc0cdacce96ef46b7848510dc8f717ae558ea564
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "38000168"
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
    IsReminderOn = true
};

await graphClient.Me.Events["{id}"]
    .Request()
    .UpdateAsync(@event);

```