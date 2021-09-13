---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ebb98c44df7f87c667759fbafb811a3355c6c7553fcaf187e4d221356b9e8d24
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274436"
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

await graphClient.Teams["{team-id}"].Schedule.TimesOff
    .Request()
    .AddAsync(timeOff);

```