---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99874cf2591b980f2aa52377f366f1145772b7402b9c5081f3b95dc3d1ab64ad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218909"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTask = new OutlookTask
{
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