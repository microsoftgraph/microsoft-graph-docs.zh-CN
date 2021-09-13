---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7a2c6865d986b05dee2fe8a0ae488de91459ef1bfbc42e49bcd5fc8cc9bf53e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219324"
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