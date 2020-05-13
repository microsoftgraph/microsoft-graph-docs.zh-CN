---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e79afc336049b632fe8ef51ca9b0ad5b8a5c106c
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "36845939"
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

await graphClient.Teams["{teamId}"].Schedule.TimesOff["{timeOffId}"]
    .Request()
    .Header("Prefer","return=representation")
    .PutAsync(timeOff);

```