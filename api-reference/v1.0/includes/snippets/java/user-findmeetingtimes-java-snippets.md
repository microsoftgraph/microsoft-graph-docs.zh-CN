---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89e1e65d9e0b04ddb2945e0bc091519957f74fe9
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983825"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "outlook.timezone=\"Pacific Standard Time\""));

LinkedList<AttendeeBase> attendeesList = new LinkedList<AttendeeBase>();
AttendeeBase attendees = new AttendeeBase();
attendees.type = AttendeeType.REQUIRED;
EmailAddress emailAddress = new EmailAddress();
emailAddress.name = "Alex Wilbur";
emailAddress.address = "alexw@contoso.onmicrosoft.com";
attendees.emailAddress = emailAddress;

attendeesList.add(attendees);

LocationConstraint locationConstraint = new LocationConstraint();
locationConstraint.isRequired = false;
locationConstraint.suggestLocation = false;
LinkedList<LocationConstraintItem> locationsList = new LinkedList<LocationConstraintItem>();
LocationConstraintItem locations = new LocationConstraintItem();
locations.resolveAvailability = false;
locations.displayName = "Conf room Hood";
locationsList.add(locations);
locationConstraint.locations = locationsList;

TimeConstraint timeConstraint = new TimeConstraint();
timeConstraint.activityDomain = ActivityDomain.WORK;
LinkedList<TimeSlot> timeSlotsList = new LinkedList<TimeSlot>();
TimeSlot timeSlots = new TimeSlot();
DateTimeTimeZone start = new DateTimeTimeZone();
start.dateTime = "2019-04-16T09:00:00";
start.timeZone = "Pacific Standard Time";
timeSlots.start = start;
DateTimeTimeZone end = new DateTimeTimeZone();
end.dateTime = "2019-04-18T17:00:00";
end.timeZone = "Pacific Standard Time";
timeSlots.end = end;
timeSlotsList.add(timeSlots);
timeConstraint.timeSlots = timeSlotsList;

boolean isOrganizerOptional = false;

Duration meetingDuration = DatatypeFactory.newInstance().newDuration("PT1H");

boolean returnSuggestionReasons = true;

Double minimumAttendeePercentage = 100d;

graphClient.me()
    .findMeetingTimes(attendeesList,locationConstraint,timeConstraint,meetingDuration,null,isOrganizerOptional,returnSuggestionReasons,minimumAttendeePercentage)
    .buildRequest( requestOptions )
    .post();

```