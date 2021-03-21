---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c26a2380ec43add82fefd217071c2896f309cf82
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982976"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Event event = new Event();
event.subject = "Let's go for lunch";
ItemBody body = new ItemBody();
body.contentType = BodyType.HTML;
body.content = "Does noon time work for you?";
event.body = body;
DateTimeTimeZone start = new DateTimeTimeZone();
start.dateTime = "2017-09-04T12:00:00";
start.timeZone = "Pacific Standard Time";
event.start = start;
DateTimeTimeZone end = new DateTimeTimeZone();
end.dateTime = "2017-09-04T14:00:00";
end.timeZone = "Pacific Standard Time";
event.end = end;
PatternedRecurrence recurrence = new PatternedRecurrence();
RecurrencePattern pattern = new RecurrencePattern();
pattern.type = RecurrencePatternType.WEEKLY;
pattern.interval = 1;
LinkedList<DayOfWeek> daysOfWeekList = new LinkedList<DayOfWeek>();
daysOfWeekList.add(DayOfWeek.MONDAY);
pattern.daysOfWeek = daysOfWeekList;
recurrence.pattern = pattern;
RecurrenceRange range = new RecurrenceRange();
range.type = RecurrenceRangeType.END_DATE;
range.startDate = new DateOnly(1900,1,1);
range.endDate = new DateOnly(1900,1,1);
recurrence.range = range;
event.recurrence = recurrence;
Location location = new Location();
location.displayName = "Harry's Bar";
event.location = location;
LinkedList<Attendee> attendeesList = new LinkedList<Attendee>();
Attendee attendees = new Attendee();
EmailAddress emailAddress = new EmailAddress();
emailAddress.address = "AdeleV@contoso.onmicrosoft.com";
emailAddress.name = "Adele Vance";
attendees.emailAddress = emailAddress;
attendees.type = AttendeeType.REQUIRED;
attendeesList.add(attendees);
event.attendees = attendeesList;

graphClient.me().events()
    .buildRequest()
    .post(event);

```