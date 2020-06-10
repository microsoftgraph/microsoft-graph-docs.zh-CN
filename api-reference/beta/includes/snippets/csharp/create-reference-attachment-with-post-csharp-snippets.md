---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4562214cdafdac41d374e09e3e4f90033c60ffc9
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684700"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var post = new Post
{
    Body = new ItemBody
    {
        ContentType = BodyType.Text,
        Content = "I attached a reference to a file on OneDrive."
    },
    Attachments = (IPostAttachmentsCollectionPage)new List<Attachment>()
    {
        new ReferenceAttachment
        {
            Name = "Personal pictures",
            SourceUrl = "https://contoso.com/personal/mario_contoso_net/Documents/Pics",
            ProviderType = ReferenceAttachmentProvider.OneDriveConsumer,
            Permission = ReferenceAttachmentPermission.Edit,
            IsFolder = true
        }
    }
};

await graphClient.Groups["1848753d-185d-4c08-a4e4-6ee40521d115"].Threads["AAQkADJUdfolA=="]
    .Reply(post)
    .Request()
    .PostAsync();

```