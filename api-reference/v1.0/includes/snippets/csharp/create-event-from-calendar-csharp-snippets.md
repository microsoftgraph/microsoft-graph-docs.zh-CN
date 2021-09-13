---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3d11a7d601abc995da363244f20ae651ee0e451cfd743e41e9836825bb546df
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163026"
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

await graphClient.Me.Calendars["{calendar-id}"].Events
    .Request()
    .AddAsync(@event);

```