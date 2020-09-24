---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b55d032d0cd99a0de37f6fda09a00ecaa3c07731
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48230707"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = new Event
{
    Subject = "Let's go for lunch",
    Body = new ItemBody
    {
        ContentType = BodyType.Html,
        Content = "Does mid month work for you?"
    },
    Start = new DateTimeTimeZone
    {
        DateTime = "2019-03-15T12:00:00",
        TimeZone = "Pacific Standard Time"
    },
    End = new DateTimeTimeZone
    {
        DateTime = "2019-03-15T14:00:00",
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
    },
    TransactionId = "7E163156-7762-4BEB-A1C6-729EA81755A7"
};

await graphClient.Me.Calendars["AAMkAGViNDU7zAAAAAGtlAAA="].Events
    .Request()
    .AddAsync(@event);

```