---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0fed1558dd65889ad17ca593ad3caf5caef0cef1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130108"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var baseTask = new BaseTask
{
    Body = new ItemBody
    {
    },
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
    PersonalProperties = new PersonalTaskProperties
    {
    }
};

await graphClient.Me.Tasks.Lists["{baseTaskList-id}"].Tasks
    .Request()
    .AddAsync(baseTask);

```