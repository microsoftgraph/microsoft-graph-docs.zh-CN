---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 837f5bf96d2672c8094970a7bb97effa90e56c26
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774290"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTask = new OutlookTask
{
    Subject = "Shop for dinner",
    StartDateTime = new DateTimeTimeZone
    {
        DateTime = "2016-04-23T18:00:00",
        TimeZone = "Pacific Standard Time"
    },
    DueDateTime = new DateTimeTimeZone
    {
        DateTime = "2016-04-25T13:00:00",
        TimeZone = "Pacific Standard Time"
    }
};

await graphClient.Me.Outlook.TaskFolders["{outlookTaskFolder-id}"].Tasks
    .Request()
    .AddAsync(outlookTask);

```