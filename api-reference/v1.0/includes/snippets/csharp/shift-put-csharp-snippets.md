---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1fbcc4dabf0c7c7e512b9166d8008d781e142073
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803441"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var shift = new Shift
{
    Id = "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
    CreatedDateTime = DateTimeOffset.Parse("2019-03-14T04:32:51.451Z"),
    LastModifiedDateTime = DateTimeOffset.Parse("2019-03-14T05:32:51.451Z"),
    UserId = "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    SchedulingGroupId = "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
    LastModifiedBy = new IdentitySet
    {
        Application = null,
        Device = null,
        User = new Identity
        {
            Id = "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
            DisplayName = "John Doe"
        },
        AdditionalData = new Dictionary<string, object>()
        {
            {"conversation", "null"}
        }
    },
    SharedShift = new ShiftItem
    {
        DisplayName = "Day shift",
        Notes = "Please do inventory as part of your shift.",
        StartDateTime = DateTimeOffset.Parse("2019-03-11T15:00:00Z"),
        EndDateTime = DateTimeOffset.Parse("2019-03-12T00:00:00Z"),
        Theme = ScheduleEntityTheme.Blue,
        Activities = new List<ShiftActivity>()
        {
            new ShiftActivity
            {
                IsPaid = true,
                StartDateTime = DateTimeOffset.Parse("2019-03-11T15:00:00Z"),
                EndDateTime = DateTimeOffset.Parse("2019-03-11T15:15:00Z"),
                Code = "",
                DisplayName = "Lunch"
            }
        }
    },
    DraftShift = new ShiftItem
    {
        DisplayName = "Day shift",
        Notes = "Please do inventory as part of your shift.",
        StartDateTime = DateTimeOffset.Parse("2019-03-11T15:00:00Z"),
        EndDateTime = DateTimeOffset.Parse("2019-03-12T00:00:00Z"),
        Theme = ScheduleEntityTheme.Blue,
        Activities = new List<ShiftActivity>()
        {
            new ShiftActivity
            {
                IsPaid = true,
                StartDateTime = DateTimeOffset.Parse("2019-03-11T15:00:00Z"),
                EndDateTime = DateTimeOffset.Parse("2019-03-11T15:30:00Z"),
                Code = "",
                DisplayName = "Lunch"
            }
        }
    }
};

await graphClient.Teams["{team-id}"].Schedule.Shifts["{shift-id}"]
    .Request()
    .Header("Prefer","return=representation")
    .UpdateAsync(shift);

```