---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c37a042068c76be3d3f97bb0f669e0e42aabcb1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885692"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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
LinkedList<String> daysOfWeekList = new LinkedList<String>();
daysOfWeekList.add("Monday");
pattern.daysOfWeek = daysOfWeekList;
recurrence.pattern = pattern;
RecurrenceRange range = new RecurrenceRange();
range.type = RecurrenceRangeType.END_DATE;
range.startDate = "2017-09-04";
range.endDate = "2017-12-31";
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