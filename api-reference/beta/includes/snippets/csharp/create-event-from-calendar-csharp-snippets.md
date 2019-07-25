---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1e8c162fa797ebd03f5a3986a6f2eb02d90266c7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709173"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = new Event
{
    Subject = "Let's go for lunch",
    Body = new ItemBody
    {
        ContentType = BodyType.Html,
        Content = "Does next month work for you?"
    },
    Start = new DateTimeTimeZone
    {
        DateTime = "2019-03-10T12:00:00",
        TimeZone = "Pacific Standard Time"
    },
    End = new DateTimeTimeZone
    {
        DateTime = "2019-03-10T14:00:00",
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
                Address = "adelev@contoso.onmicrosoft.com",
                Name = "Adele Vance"
            },
            Type = AttendeeType.Required
        }
    }
};

await graphClient.Me.Calendars["AAMkAGViNDU7zAAAAAGtlAAA="].Events
    .Request()
    .AddAsync(@event);

```