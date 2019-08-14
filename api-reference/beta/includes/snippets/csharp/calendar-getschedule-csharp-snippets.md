---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6e0b178a6b69850e1027588c60845b66cc417fd
ms.sourcegitcommit: 3db93e28e215c0e09a65b4705ba956c6ac3b5426
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/14/2019
ms.locfileid: "36396707"
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

var availabilityViewInterval = 60;

await graphClient.Me.Calendar
    .GetSchedule(schedules,endTime,startTime,availabilityViewInterval)
    .Request()
    .Header("Prefer","outlook.timezone=\"Pacific Standard Time\"")
    .PostAsync();

```