---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 371ba1176e4bde78cd7d16f831b202460013c18fe4a3db273221d64fa6551481
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334045"
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