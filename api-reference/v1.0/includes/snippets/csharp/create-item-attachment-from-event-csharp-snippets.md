---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0381b83c768084c47600c65ef6a7ac6d787a622f
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473817"
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
            DateTime = "2016-12-02T18:00:00",
            TimeZone = "Pacific Standard Time"
        },
        End = new DateTimeTimeZone
        {
            DateTime = "2016-12-02T19:00:00",
            TimeZone = "Pacific Standard Time"
        }
    }
};

await graphClient.Me.Events["AAMkAGI1AAAt9AHjAAA="].Attachments
    .Request()
    .AddAsync(attachment);

```