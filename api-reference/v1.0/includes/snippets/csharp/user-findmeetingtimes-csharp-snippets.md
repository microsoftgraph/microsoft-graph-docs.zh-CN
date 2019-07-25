---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f0c9b51a2872435dcbc8a68312d552cbb1f29ea7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715060"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attendees = new List<AttendeeBase>()
{
    new AttendeeBase
    {
        Type = AttendeeType.Required,
        EmailAddress = new EmailAddress
        {
            Name = "Alex Wilbur",
            Address = "alexw@contoso.onmicrosoft.com"
        }
    }
};

var locationConstraint = new LocationConstraint
{
    IsRequired = "false",
    SuggestLocation = "false",
    Locations = new List<LocationConstraintItem>()
    {
        new LocationConstraintItem
        {
            ResolveAvailability = "false",
            DisplayName = "Conf room Hood"
        }
    }
};

var timeConstraint = new TimeConstraint
{
    ActivityDomain = ActivityDomain.Work,
    Timeslots = new List<TimeSlot>()
    {
        new TimeSlot
        {
            Start = new DateTimeTimeZone
            {
                DateTime = "2019-04-16T09:00:00",
                TimeZone = "Pacific Standard Time"
            },
            End = new DateTimeTimeZone
            {
                DateTime = "2019-04-18T17:00:00",
                TimeZone = "Pacific Standard Time"
            }
        }
    }
};

var isOrganizerOptional = false;

var meetingDuration = "PT1H";

var returnSuggestionReasons = true;

var minimumAttendeePercentage = "100";

await graphClient.Me
    .FindMeetingTimes(attendees,locationConstraint,timeConstraint,meetingDuration,maxCandidates,isOrganizerOptional,returnSuggestionReasons,minimumAttendeePercentage)
    .Request()
    .Header("Prefer","outlook.timezone=\"Pacific Standard Time\"")
    .PostAsync();

```