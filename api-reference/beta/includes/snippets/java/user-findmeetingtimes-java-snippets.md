---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1ba15a7c10a5755d8e03b3b5c18f95353ac733e9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867789"
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
    .findMeetingTimes(attendeesList,locationConstraint,timeConstraint,meetingDuration,maxCandidates,isOrganizerOptional,returnSuggestionReasons,minimumAttendeePercentage)
    .buildRequest( requestOptions )
    .post();

```