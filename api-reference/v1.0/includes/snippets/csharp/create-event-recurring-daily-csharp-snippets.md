---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c4aabc09d55e7804e5fe02626a59783cf08e0387
ms.sourcegitcommit: d419565add1f731be50c9b5911eb1310fa007097
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2020
ms.locfileid: "42280710"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = new Event
{
    Subject = "Let's go for lunch",
    Body = new ItemBody
    {
        ContentType = BodyType.Html,
        Content = "Does noon work for you?"
    },
    Start = new DateTimeTimeZone
    {
        DateTime = "2020-02-21T12:00:00",
        TimeZone = "Pacific Standard Time"
    },
    End = new DateTimeTimeZone
    {
        DateTime = "2020-02-21T14:00:00",
        TimeZone = "Pacific Standard Time"
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
                Address = "AlexW@contoso.OnMicrosoft.com",
                Name = "Alex Wilbur"
            },
            Type = AttendeeType.Required
        }
    },
    Recurrence = new PatternedRecurrence
    {
        Pattern = new RecurrencePattern
        {
            Type = RecurrencePatternType.Daily,
            Interval = 1
        },
        Range = new RecurrenceRange
        {
            Type = RecurrenceRangeType.Numbered,
            StartDate = new Date(2020,2,21),
            NumberOfOccurrences = 2
        }
    }
};

await graphClient.Me.Events
    .Request()
    .Header("Prefer","outlook.timezone=\"Pacific Standard Time\"")
    .AddAsync(@event);

```