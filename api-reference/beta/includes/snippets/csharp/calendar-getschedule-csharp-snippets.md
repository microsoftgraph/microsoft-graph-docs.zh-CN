---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0e35838a141ad35f10212b33fa1e1159370bd23ba0baa02c214b88c765b5c3e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161899"
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