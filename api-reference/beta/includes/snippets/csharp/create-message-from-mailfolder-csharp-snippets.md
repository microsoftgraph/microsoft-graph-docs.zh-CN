---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c458b671699e66b0cd32c4117e07f6dd6e74a54f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721549"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    ReceivedDateTime = "2016-10-19T10:37:00Z",
    SentDateTime = "2016-10-19T10:37:00Z",
    HasAttachments = true,
    Subject = "subject-value",
    Body = new ItemBody
    {
        ContentType = BodyType.Text,
        Content = "content-value"
    },
    BodyPreview = "bodyPreview-value"
};

await graphClient.Me.MailFolders["{id}"].Messages
    .Request()
    .AddAsync(message);

```