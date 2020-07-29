---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 112f3aa17b658e621a22e65af44aef828ba96497
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46512145"
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
    },
    AllowNewTimeProposals = true
};

await graphClient.Me.Events
    .Request()
    .AddAsync(@event);

```