---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 69651d05bc402181a04231e4796de074f8652f32
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730239"
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