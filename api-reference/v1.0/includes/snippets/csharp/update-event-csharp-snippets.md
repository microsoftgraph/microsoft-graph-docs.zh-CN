---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9fc204b2cd85b1b46ee3cede0173ab5591d13bd9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730222"
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
        Time = "datetime-value"
    },
    Recurrence = null,
    ICalUId = "iCalUId-value",
    ReminderMinutesBeforeStart = 99,
    IsReminderOn = true
};

await graphClient.Me.Events["{id}"]
    .Request()
    .UpdateAsync(@event);

```