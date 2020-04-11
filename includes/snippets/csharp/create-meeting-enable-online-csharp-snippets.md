---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72815bebed6d1d8604cc0a9852b0aa59f0842cd0
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636961"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = new Event
{
    Subject = "Prep for customer meeting",
    Body = new ItemBody
    {
        ContentType = BodyType.Html,
        Content = "Does this time work for you?"
    },
    Start = new DateTimeTimeZone
    {
        DateTime = "2019-11-20T13:00:00",
        TimeZone = "Pacific Standard Time"
    },
    End = new DateTimeTimeZone
    {
        DateTime = "2019-11-20T14:00:00",
        TimeZone = "Pacific Standard Time"
    },
    Location = new Location
    {
        DisplayName = "Cordova conference room"
    },
    Attendees = new List<Attendee>()
    {
        new Attendee
        {
            EmailAddress = new EmailAddress
            {
                Address = "AdeleV@contoso.OnMicrosoft.com",
                Name = "Adele Vance"
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