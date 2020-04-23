---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 70d5fe31620d46def74d41b0497b2c93a1bdfe09
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43771146"
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

await graphClient.Me.Calendars["AAMkAGViNDU9zAAAAAGtlAAA="].Events
    .Request()
    .AddAsync(@event);

```