---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b8b8a187fd6a3ad627718d07c2a2aebd8ddea5fa
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791352"
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
    },
    IsOnlineMeeting = true,
    OnlineMeetingProvider = OnlineMeetingProviderType.TeamsForBusiness
};

await graphClient.Me.Calendars["{calendar-id}"].Events
    .Request()
    .AddAsync(@event);

```