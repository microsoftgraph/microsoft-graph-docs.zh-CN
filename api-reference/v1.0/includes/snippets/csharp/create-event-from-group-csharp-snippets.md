---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79c91771f99c4db4a6c171875ef462b206a6e109
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789014"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = new Event
{
    Subject = "Let's go for lunch",
    Body = new ItemBody
    {
        ContentType = BodyType.Html,
        Content = "Does late morning work for you?"
    },
    Start = new DateTimeTimeZone
    {
        DateTime = "2019-06-16T12:00:00",
        TimeZone = "Pacific Standard Time"
    },
    End = new DateTimeTimeZone
    {
        DateTime = "2019-06-16T14:00:00",
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

await graphClient.Groups["{group-id}"].Events
    .Request()
    .AddAsync(@event);

```