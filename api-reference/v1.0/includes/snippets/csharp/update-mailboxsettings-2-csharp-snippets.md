---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2887610cbda7e23ce505aa379fd6cfd52638558c17a5206d5336940d9864dd69
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904061"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailboxSettings = new MailboxSettings
{
    WorkingHours = new WorkingHours
    {
        EndTime = new TimeOfDay(18, 30, 0),
        DaysOfWeek = new List<DayOfWeek>()
        {
            DayOfWeek.Monday,
            DayOfWeek.Tuesday,
            DayOfWeek.Wednesday,
            DayOfWeek.Thursday,
            DayOfWeek.Friday,
            DayOfWeek.Saturday
        },
        TimeZone = new CustomTimeZone
        {
            Bias = -300,
            Name = "Customized Time Zone",
            StandardOffset = new StandardTimeZoneOffset
            {
                Time = new TimeOfDay(2, 0, 0),
                DayOccurrence = 2,
                DayOfWeek = DayOfWeek.Sunday,
                Month = 10,
                Year = 0
            },
            DaylightOffset = new DaylightTimeZoneOffset
            {
                DaylightBias = 100,
                Time = new TimeOfDay(2, 0, 0),
                DayOccurrence = 4,
                DayOfWeek = DayOfWeek.Sunday,
                Month = 5,
                Year = 0
            }
        }
    }
};

var me = new User();
me.MailboxSettings = mailboxSettings;

await graphClient.Me
    .Request()
    .UpdateAsync(me);

```