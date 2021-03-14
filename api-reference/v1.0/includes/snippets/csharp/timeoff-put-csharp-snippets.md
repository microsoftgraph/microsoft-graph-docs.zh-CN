---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a217428b5ed4c21e246eea836df2189410cd401
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793042"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeOff = new TimeOff
{
    UserId = "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    SharedTimeOff = new TimeOffItem
    {
        TimeOffReasonId = "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
        StartDateTime = DateTimeOffset.Parse("2019-03-11T07:00:00Z"),
        EndDateTime = DateTimeOffset.Parse("2019-03-12T07:00:00Z"),
        Theme = ScheduleEntityTheme.White
    },
    DraftTimeOff = new TimeOffItem
    {
        TimeOffReasonId = "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
        StartDateTime = DateTimeOffset.Parse("2019-03-11T07:00:00Z"),
        EndDateTime = DateTimeOffset.Parse("2019-03-12T07:00:00Z"),
        Theme = ScheduleEntityTheme.Pink
    }
};

await graphClient.Teams["{team-id}"].Schedule.TimesOff["{timeOff-id}"]
    .Request()
    .Header("Prefer","return=representation")
    .PutAsync(timeOff);

```