---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 729d9b8c882760599b40ce86d0e021763388f0d7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478767"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeOff = new TimeOff
{
    UserId = "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    SharedTimeOff = new TimeOffItem
    {
        TimeOffReasonId = "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
        StartDateTime = "2019-03-11T07:00:00Z",
        EndDateTime = "2019-03-12T07:00:00Z",
        Theme = ScheduleEntityTheme.White
    },
    DraftTimeOff = new TimeOffItem
    {
        TimeOffReasonId = "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
        StartDateTime = "2019-03-11T07:00:00Z",
        EndDateTime = "2019-03-12T07:00:00Z",
        Theme = ScheduleEntityTheme.Pink
    }
};

await graphClient.Teams["{teamId}"].Schedule.TimesOff["{timeOffId}"]
    .Request()
    .Header("Prefer","return=representation")
    .PutAsync(timeOff);

```