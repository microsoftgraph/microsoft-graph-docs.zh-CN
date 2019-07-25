---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7e06954ee3c50dee067592fc3b54a523324b3656
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714073"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var newReminderTime = new DateTimeTimeZone
{
    DateTime = "2016-10-19T10:37:00Z",
    TimeZone = "timeZone-value"
};

await graphClient.Me.Events["{id}"]
    .SnoozeReminder(newReminderTime)
    .Request()
    .PostAsync();

```