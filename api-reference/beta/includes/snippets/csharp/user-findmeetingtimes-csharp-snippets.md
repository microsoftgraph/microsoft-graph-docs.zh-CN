---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd24fcc4705fd082f058ade1269bb18c06f675a7
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683742"
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
    IsRequired = false,
    SuggestLocation = false,
    Locations = new List<LocationConstraintItem>()
    {
        new LocationConstraintItem
        {
            ResolveAvailability = false,
            DisplayName = "Conf room Hood"
        }
    }
};

var timeConstraint = new TimeConstraint
{
    ActivityDomain = ActivityDomain.Work,
    TimeSlots = new List<TimeSlot>()
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

var meetingDuration = new Duration("PT1H");

var returnSuggestionReasons = true;

var minimumAttendeePercentage = (double)100;

await graphClient.Me
    .FindMeetingTimes(attendees,locationConstraint,timeConstraint,meetingDuration,null,isOrganizerOptional,returnSuggestionReasons,minimumAttendeePercentage)
    .Request()
    .Header("Prefer","outlook.timezone=\"Pacific Standard Time\"")
    .PostAsync();

```