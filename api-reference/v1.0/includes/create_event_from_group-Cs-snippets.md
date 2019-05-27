---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 679ed05a83e894fbfe2bfb4c6da6a1b213df7bae
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440385"
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
    ICalUId = "iCalUId-value",
    ReminderMinutesBeforeStart = 99,
    IsReminderOn = true
};

await graphClient.Groups["{id}"].Events
    .Request()
    .AddAsync(@event);

```