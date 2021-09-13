---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be358e2638d74e3ae505848b2de58dd583bfa6b75b6b52be4860ab6a69974b87
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218730"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var openShift = new OpenShift
{
    SchedulingGroupId = "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
    SharedOpenShift = new OpenShiftItem
    {
        Notes = "Inventory Management",
        OpenSlotCount = 5,
        DisplayName = "Field shift",
        StartDateTime = DateTimeOffset.Parse("2018-10-04T00:58:45.34Z"),
        EndDateTime = DateTimeOffset.Parse("2018-10-04T09:50:45.332Z"),
        Theme = ScheduleEntityTheme.White,
        Activities = new List<ShiftActivity>()
        {
            new ShiftActivity
            {
                IsPaid = true,
                StartDateTime = DateTimeOffset.Parse("2018-10-04T00:58:45.34Z"),
                EndDateTime = DateTimeOffset.Parse("2018-10-04T01:58:45.34Z"),
                Code = "",
                DisplayName = "Lunch"
            }
        }
    },
    DraftOpenShift = null
};

await graphClient.Teams["{team-id}"].Schedule.OpenShifts["{openShift-id}"]
    .Request()
    .UpdateAsync(openShift);

```