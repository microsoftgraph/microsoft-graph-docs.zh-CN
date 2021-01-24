---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5bb13f29b76a2c80212e4894b6fec1236d32b403
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946046"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var post = new Post
{
    Body = new ItemBody
    {
        ContentType = BodyType.Text,
        Content = "I attached an event."
    },
    Attachments = new PostAttachmentsCollectionPage()
    {
        new ItemAttachment
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
                    DateTime = "2019-12-02T18:00:00",
                    TimeZone = "Pacific Standard Time"
                },
                End = new DateTimeTimeZone
                {
                    DateTime = "2019-12-02T19:00:00",
                    TimeZone = "Pacific Standard Time"
                }
            }
        }
    }
};

await graphClient.Groups["1848753d-185d-4c08-a4e4-6ee40521d115"].Threads["AAQkADJUdfolA=="]
    .Reply(post)
    .Request()
    .PostAsync();

```