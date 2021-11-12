---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f692d08000924de7e2b18a95ca16864fd79e93bdc355b343bfbf3379d31fa61a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333602"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = new Event
{
    Subject = "Let's go for lunch",
    Body = new ItemBody
    {
        ContentType = BodyType.Html,
        Content = "Does noon time work for you?"
    },
    Start = new DateTimeTimeZone
    {
        DateTime = "2017-09-04T12:00:00",
        TimeZone = "Pacific Standard Time"
    },
    End = new DateTimeTimeZone
    {
        DateTime = "2017-09-04T14:00:00",
        TimeZone = "Pacific Standard Time"
    },
    Recurrence = new PatternedRecurrence
    {
        Pattern = new RecurrencePattern
        {
            Type = RecurrencePatternType.Weekly,
            Interval = 1,
            DaysOfWeek = new List<DayOfWeek>()
            {
                DayOfWeek.Monday
            }
        },
        Range = new RecurrenceRange
        {
            Type = RecurrenceRangeType.EndDate,
            StartDate = new Date(2017,9,4),
            EndDate = new Date(2017,12,31)
        }
    },
    Location = new Location
    {
        DisplayName = "Harry's Bar"
    },
    Attendees = new List<Attendee>()
    {
        new Attendee
        {
            EmailAddress = new EmailAddress
            {
                Address = "AdeleV@contoso.onmicrosoft.com",
                Name = "Adele Vance"
            },
            Type = AttendeeType.Required
        }
    }
};

await graphClient.Me.Events
    .Request()
    .AddAsync(@event);

```