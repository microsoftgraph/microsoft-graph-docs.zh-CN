---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d28450a838b1ec4c90de2b8a12c0884a1bfc7215
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536909"
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
            DaysOfWeek = new List<String>()
            {
                "Monday"
            }
        },
        Range = new RecurrenceRange
        {
            Type = RecurrenceRangeType.EndDate,
            StartDate = "2017-09-04",
            EndDate = "2017-12-31"
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