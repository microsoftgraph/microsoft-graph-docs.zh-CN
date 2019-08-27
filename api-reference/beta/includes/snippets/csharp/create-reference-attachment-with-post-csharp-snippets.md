---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7faebd89f9e8823c9b56443db6d8cd994923a2f9
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633543"
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
    Attachments = new List<Attachment>()
    {
        new Attachment
        {
            AdditionalData = new Dictionary<string, object>()
            {
                {"@odata.type","#microsoft.graph.referenceAttachment"}
            },
            Name = "Personal pictures",
            SourceUrl = "https://contoso.com/personal/mario_contoso_net/Documents/Pics",
            ProviderType = "oneDriveConsumer",
            Permission = "Edit",
            IsFolder = "True"
        }
    }
};

await graphClient.Groups["1848753d-185d-4c08-a4e4-6ee40521d115"].Threads["AAQkADJUdfolA=="]
    .Reply(post)
    .Request()
    .PostAsync();

```