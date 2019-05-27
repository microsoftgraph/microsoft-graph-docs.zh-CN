---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c74e5800730c8795a988af5856fdf6b72bc456b7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480538"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var shift = new Shift
{
    Id = "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
    UserId = "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    SchedulingGroupId = "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
    SharedShift = new ShiftItem
    {
        DisplayName = "Day shift",
        Notes = "Please do inventory as part of your shift.",
        StartDateTime = "2019-03-11T15:00:00Z",
        EndDateTime = "2019-03-12T00:00:00Z",
        Theme = ScheduleEntityTheme.Blue,
        Activities = new List<ShiftActivity>()
        {
            new ShiftActivity
            {
                IsPaid = true,
                StartDateTime = "2019-03-11T15:00:00Z",
                EndDateTime = "2019-03-11T15:15:00Z",
                Code = "",
                DisplayName = "Lunch"
            }
        }
    },
    DraftShift = new ShiftItem
    {
        DisplayName = "Day shift",
        Notes = "Please do inventory as part of your shift.",
        StartDateTime = "2019-03-11T15:00:00Z",
        EndDateTime = "2019-03-12T00:00:00Z",
        Theme = ScheduleEntityTheme.Blue,
        Activities = new List<ShiftActivity>()
        {
            new ShiftActivity
            {
                IsPaid = true,
                StartDateTime = "2019-03-11T15:00:00Z",
                EndDateTime = "2019-03-11T15:30:00Z",
                Code = "",
                DisplayName = "Lunch"
            }
        }
    }
};

await graphClient.Teams["{teamId}"].Schedule.Shifts
    .Request()
    .AddAsync(shift);

```