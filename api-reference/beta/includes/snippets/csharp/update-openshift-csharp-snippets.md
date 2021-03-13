---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e46e5fdd065f9fe3efb367d09f7cc1f18892eef2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798356"
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
    .PutAsync(openShift);

```