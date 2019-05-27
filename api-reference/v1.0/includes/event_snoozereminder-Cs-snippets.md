---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 69651d05bc402181a04231e4796de074f8652f32
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457701"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var newReminderTime = new DateTimeTimeZone
{
    DateTime = "dateTime-value",
    TimeZone = "timeZone-value"
};

await graphClient.Me.Events["{id}"]
    .SnoozeReminder(newReminderTime)
    .Request()
    .PostAsync();

```