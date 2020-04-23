---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b41c44a10490996889095b50ba0e6fd7fa746b57
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43771086"
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
        DateTime = "2017-04-15T12:00:00",
        TimeZone = "Pacific Standard Time"
    },
    End = new DateTimeTimeZone
    {
        DateTime = "2017-04-15T14:00:00",
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
                Address = "samanthab@contoso.onmicrosoft.com",
                Name = "Samantha Booth"
            },
            Type = AttendeeType.Required
        }
    },
    AllowNewTimeProposals = true,
    IsOnlineMeeting = true,
    OnlineMeetingProvider = OnlineMeetingProviderType.TeamsForBusiness
};

await graphClient.Me.Events
    .Request()
    .Header("Prefer","outlook.timezone=\"Pacific Standard Time\"")
    .AddAsync(@event);

```