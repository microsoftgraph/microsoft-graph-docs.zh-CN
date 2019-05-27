---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 796b1d9aef3ac56745a70da4c79945a3530a3cb0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440098"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTask = new OutlookTask
{
    AssignedTo = "Dana Swope",
    Subject = "Shop for children's weekend",
    StartDateTime = new DateTimeTimeZone
    {
        DateTime = "2016-05-03T09:00:00",
        TimeZone = "Eastern Standard Time"
    },
    DueDateTime = new DateTimeTimeZone
    {
        DateTime = "2016-05-05T16:00:00",
        TimeZone = "Eastern Standard Time"
    }
};

await graphClient.Me.Outlook.Tasks
    .Request()
    .Header("Prefer","outlook.timezone=\"Pacific Standard Time\"")
    .AddAsync(outlookTask);

```