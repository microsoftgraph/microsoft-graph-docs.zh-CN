---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82c820635ff3fe0bf18a46bc8092b6e857268717e2ddde7c5f111ff04c1d41f3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104021"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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

graphClient.me().calendars("AAMkAGViNDU8zAAAAAGtlAAA=").events()
    .buildRequest()
    .post(event);

```