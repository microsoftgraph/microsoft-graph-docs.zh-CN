---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90b451841ded470751c569e471c0fd5fe85daa26
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2020
ms.locfileid: "44384303"
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

await graphClient.Teams["{id}"].Schedule.OpenShifts["OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8"]
    .Request()
    .UpdateAsync(openShift);

```