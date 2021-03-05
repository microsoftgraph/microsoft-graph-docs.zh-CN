---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85712607594dd46b2b19d01e442b42046ee19563
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474756"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new ItemAttachment
{
    Name = "Holiday event",
    Item = new Event
    {
        Subject = "Discuss gifts for children",
        Body = new ItemBody
        {
            ContentType = BodyType.Html,
            Content = "Let's look for funding!"
        },
        Start = new DateTimeTimeZone
        {
            DateTime = "2020-01-12T18:00:00",
            TimeZone = "Pacific Standard Time"
        },
        End = new DateTimeTimeZone
        {
            DateTime = "2020-01-12T19:00:00",
            TimeZone = "Pacific Standard Time"
        }
    }
};

await graphClient.Me.Outlook.Tasks["AAMkADAAAANXbdnAAA="].Attachments
    .Request()
    .AddAsync(attachment);

```