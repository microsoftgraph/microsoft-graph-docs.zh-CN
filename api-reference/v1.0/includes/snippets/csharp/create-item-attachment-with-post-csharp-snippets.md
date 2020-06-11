---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4fd2133b042f67962f10fb359831bdd113c38ce
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44682062"
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
    Attachments = (IPostAttachmentsCollectionPage)new List<Attachment>()
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