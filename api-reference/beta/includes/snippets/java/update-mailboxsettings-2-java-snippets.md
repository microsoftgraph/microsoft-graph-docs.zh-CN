---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06b4c6c3f0560c67fcc2ffc6185102714a179add
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475021"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailboxSettings mailboxSettings = new MailboxSettings();
WorkingHours workingHours = new WorkingHours();
workingHours.endTime = new TimeOfDay(0, 0, 0);
LinkedList<DayOfWeek> daysOfWeekList = new LinkedList<DayOfWeek>();
daysOfWeekList.add(DayOfWeek.MONDAY);
daysOfWeekList.add(DayOfWeek.TUESDAY);
daysOfWeekList.add(DayOfWeek.WEDNESDAY);
daysOfWeekList.add(DayOfWeek.THURSDAY);
daysOfWeekList.add(DayOfWeek.FRIDAY);
daysOfWeekList.add(DayOfWeek.SATURDAY);
workingHours.daysOfWeek = daysOfWeekList;
CustomTimeZone timeZone = new CustomTimeZone();
timeZone.bias = -300;
timeZone.name = "Customized Time Zone";
StandardTimeZoneOffset standardOffset = new StandardTimeZoneOffset();
standardOffset.time = new TimeOfDay(0, 0, 0);
standardOffset.dayOccurrence = 2;
standardOffset.dayOfWeek = DayOfWeek.SUNDAY;
standardOffset.month = 10;
standardOffset.year = 0;
timeZone.standardOffset = standardOffset;
DaylightTimeZoneOffset daylightOffset = new DaylightTimeZoneOffset();
daylightOffset.daylightBias = 100;
daylightOffset.time = new TimeOfDay(0, 0, 0);
daylightOffset.dayOccurrence = 4;
daylightOffset.dayOfWeek = DayOfWeek.SUNDAY;
daylightOffset.month = 5;
daylightOffset.year = 0;
timeZone.daylightOffset = daylightOffset;
workingHours.timeZone = timeZone;
mailboxSettings.workingHours = workingHours;

graphClient.customRequest("/me/mailboxSettings", MailboxSettings.class)
    .buildRequest()
    .patch(mailboxSettings);

```