---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a90aa217c7db683d9bf245ad1bc0b292f5eeda51e7a630a2d03dea876e67e639
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332607"
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

await graphClient.Me.Events["{event-id}"].Attachments
    .Request()
    .AddAsync(attachment);

```