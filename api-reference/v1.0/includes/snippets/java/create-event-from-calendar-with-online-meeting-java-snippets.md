---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0fb8ed67943df71b0d218e3038268f3844290da
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43771037"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Event event = new Event();
event.subject = "Let's go for lunch";
ItemBody body = new ItemBody();
body.contentType = BodyType.HTML;
body.content = "Does next month work for you?";
event.body = body;
DateTimeTimeZone start = new DateTimeTimeZone();
start.dateTime = "2019-03-10T12:00:00";
start.timeZone = "Pacific Standard Time";
event.start = start;
DateTimeTimeZone end = new DateTimeTimeZone();
end.dateTime = "2019-03-10T14:00:00";
end.timeZone = "Pacific Standard Time";
event.end = end;
Location location = new Location();
location.displayName = "Harry's Bar";
event.location = location;
LinkedList<Attendee> attendeesList = new LinkedList<Attendee>();
Attendee attendees = new Attendee();
EmailAddress emailAddress = new EmailAddress();
emailAddress.address = "adelev@contoso.onmicrosoft.com";
emailAddress.name = "Adele Vance";
attendees.emailAddress = emailAddress;
attendees.type = AttendeeType.REQUIRED;
attendeesList.add(attendees);
event.attendees = attendeesList;
event.isOnlineMeeting = true;
event.onlineMeetingProvider = OnlineMeetingProviderType.TEAMS_FOR_BUSINESS;

graphClient.me().calendars("AAMkAGViNDU9zAAAAAGtlAAA=").events()
    .buildRequest()
    .post(event);

```