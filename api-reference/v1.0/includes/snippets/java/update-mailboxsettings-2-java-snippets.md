---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d9555e0c9ed66f1368e4de5e27ad5b0b9301abc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979720"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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