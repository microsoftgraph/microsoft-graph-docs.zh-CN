---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd68ea4aa8cead6049f37985e76a76f567d8a7d0
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475505"
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