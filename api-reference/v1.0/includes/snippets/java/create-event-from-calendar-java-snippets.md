---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e3e22bf8d7ef2c74ad01d2332350ac2de1b1f6a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882424"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Event event = new Event();
event.subject = "Let's go for lunch";
ItemBody body = new ItemBody();
body.contentType = BodyType.HTML;
body.content = "Does mid month work for you?";
event.body = body;
DateTimeTimeZone start = new DateTimeTimeZone();
start.dateTime = "2019-03-15T12:00:00";
start.timeZone = "Pacific Standard Time";
event.start = start;
DateTimeTimeZone end = new DateTimeTimeZone();
end.dateTime = "2019-03-15T14:00:00";
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

graphClient.me().calendars("AAMkAGViNDU7zAAAAAGtlAAA=").events()
    .buildRequest()
    .post(event);

```