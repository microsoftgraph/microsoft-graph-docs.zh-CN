---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec92055813b7be1c9f7ffd2b7178d4c6b078820b
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932087"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schedules = new List<String>()
{
    "adelev@contoso.onmicrosoft.com",
    "meganb@contoso.onmicrosoft.com"
};

var startTime = new DateTimeTimeZone
{
    DateTime = "2019-03-15T09:00:00",
    TimeZone = "Pacific Standard Time"
};

var endTime = new DateTimeTimeZone
{
    DateTime = "2019-03-15T18:00:00",
    TimeZone = "Pacific Standard Time"
};

var availabilityViewInterval = "60";

await graphClient.Me.Calendar
    .Getschedule(schedules,endTime,startTime,availabilityViewInterval)
    .Request()
    .Header("Prefer","outlook.timezone=\"Pacific Standard Time\"")
    .PostAsync();

```