---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3c2b2f7ea3e6f401a00c3b92500abea86a769e7
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402935"
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
locationConstraint.isRequired = "false";
locationConstraint.suggestLocation = "false";
LinkedList<LocationConstraintItem> locationsList = new LinkedList<LocationConstraintItem>();
LocationConstraintItem locations = new LocationConstraintItem();
locations.resolveAvailability = "false";
locations.displayName = "Conf room Hood";
locationsList.add(locations);
locationConstraint.locations = locationsList;

TimeConstraint timeConstraint = new TimeConstraint();
timeConstraint.activityDomain = ActivityDomain.WORK;
LinkedList<TimeSlot> timeslotsList = new LinkedList<TimeSlot>();
TimeSlot timeslots = new TimeSlot();
DateTimeTimeZone start = new DateTimeTimeZone();
start.dateTime = "2019-04-16T09:00:00";
start.timeZone = "Pacific Standard Time";
timeslots.start = start;
DateTimeTimeZone end = new DateTimeTimeZone();
end.dateTime = "2019-04-18T17:00:00";
end.timeZone = "Pacific Standard Time";
timeslots.end = end;
timeslotsList.add(timeslots);
timeConstraint.timeslots = timeslotsList;

boolean isOrganizerOptional = false;

String meetingDuration = "PT1H";

boolean returnSuggestionReasons = true;

String minimumAttendeePercentage = "100";

graphClient.me()
    .findMeetingTimes(attendeesList,locationConstraint,timeConstraint,meetingDuration,null,isOrganizerOptional,returnSuggestionReasons,minimumAttendeePercentage)
    .buildRequest( requestOptions )
    .post();

```