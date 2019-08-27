---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9d29b2bd62958b0b77e13c5e7c92f1241a580308
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633564"
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
    Attachments = new List<Attachment>()
    {
        new Attachment
        {
            AdditionalData = new Dictionary<string, object>()
            {
                {"@odata.type","#microsoft.graph.fileAttachment"}
            },
            Name = "Another file as attachment",
            ContentBytes = "VGhpcyBpcyBhIGZpbGUgdG8gYmUgYXR0YWNoZWQu"
        }
    }
};

await graphClient.Groups["1848753d-185d-4c08-a4e4-6ee40521d115"].Threads["AAQkADJUdfolA=="]
    .Reply(post)
    .Request()
    .PostAsync();

```