---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43e5b9525ae8bd9f3e10e0c585599051c8168cf3656b702e8263973d0c105800
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218636"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "outlook.timezone=\"Pacific Standard Time\""));

Event event = new Event();
event.subject = "Let's go for lunch";
ItemBody body = new ItemBody();
body.contentType = BodyType.HTML;
body.content = "Does noon work for you?";
event.body = body;
DateTimeTimeZone start = new DateTimeTimeZone();
start.dateTime = "2017-04-15T12:00:00";
start.timeZone = "Pacific Standard Time";
event.start = start;
DateTimeTimeZone end = new DateTimeTimeZone();
end.dateTime = "2017-04-15T14:00:00";
end.timeZone = "Pacific Standard Time";
event.end = end;
Location location = new Location();
location.displayName = "Harry's Bar";
event.location = location;
LinkedList<Attendee> attendeesList = new LinkedList<Attendee>();
Attendee attendees = new Attendee();
EmailAddress emailAddress = new EmailAddress();
emailAddress.address = "samanthab@contoso.onmicrosoft.com";
emailAddress.name = "Samantha Booth";
attendees.emailAddress = emailAddress;
attendees.type = AttendeeType.REQUIRED;
attendeesList.add(attendees);
event.attendees = attendeesList;
event.allowNewTimeProposals = true;
event.transactionId = "7E163156-7762-4BEB-A1C6-729EA81755A7";

graphClient.me().events()
    .buildRequest( requestOptions )
    .post(event);

```