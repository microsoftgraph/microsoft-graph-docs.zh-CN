---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 376083f2bd36ef50ef100c5f3876f732b338453c
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528103"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var baseTask = new Task
{
    TextBody = "String",
    BodyLastModifiedDateTime = DateTimeOffset.Parse("String (timestamp)"),
    CompletedDateTime = DateTimeOffset.Parse("String (timestamp)"),
    DueDateTime = new DateTimeTimeZone
    {
    },
    StartDateTime = new DateTimeTimeZone
    {
    },
    Importance = Importance.Low,
    Recurrence = new PatternedRecurrence
    {
    },
    DisplayName = "String",
    Status = TaskStatus_v2.NotStarted,
    Viewpoint = new TaskViewpoint
    {
    }
};

await graphClient.Me.Tasks.Lists["{baseTaskList-id}"].Tasks["{baseTask-id}"]
    .Request()
    .UpdateAsync(baseTask);

```