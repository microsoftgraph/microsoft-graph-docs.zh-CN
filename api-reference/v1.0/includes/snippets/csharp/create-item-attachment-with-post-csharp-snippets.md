---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4059f785131e0fb010872bcdf2acd4e8d8f32b5a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782563"
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

await graphClient.Groups["{group-id}"].Threads["{conversationThread-id}"]
    .Reply(post)
    .Request()
    .PostAsync();

```