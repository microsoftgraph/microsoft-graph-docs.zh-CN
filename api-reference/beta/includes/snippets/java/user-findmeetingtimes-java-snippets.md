---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88430e02175e13233144ae9529c12e8cc1bc794845a7e3f909f600d6e9af32ef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277396"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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
    .findMeetingTimes(UserFindMeetingTimesParameterSet
        .newBuilder()
        .withAttendees(attendeesList)
        .withLocationConstraint(locationConstraint)
        .withTimeConstraint(timeConstraint)
        .withMeetingDuration(meetingDuration)
        .withMaxCandidates(null)
        .withIsOrganizerOptional(isOrganizerOptional)
        .withReturnSuggestionReasons(returnSuggestionReasons)
        .withMinimumAttendeePercentage(minimumAttendeePercentage)
        .build())
    .buildRequest( requestOptions )
    .post();

```