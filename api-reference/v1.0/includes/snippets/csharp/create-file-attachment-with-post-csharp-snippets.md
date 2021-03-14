---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34fb0bac1f8a49202c7c10510ce8bc4f5ee8709a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807739"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var post = new Post
{
    Body = new ItemBody
    {
        ContentType = BodyType.Text,
        Content = "Which quarter does that file cover? See my attachment."
    },
    Attachments = new PostAttachmentsCollectionPage()
    {
        new FileAttachment
        {
            Name = "Another file as attachment",
            ContentBytes = Encoding.ASCII.GetBytes("VGhpcyBpcyBhIGZpbGUgdG8gYmUgYXR0YWNoZWQu")
        }
    }
};

await graphClient.Groups["{group-id}"].Threads["{conversationThread-id}"]
    .Reply(post)
    .Request()
    .PostAsync();

```