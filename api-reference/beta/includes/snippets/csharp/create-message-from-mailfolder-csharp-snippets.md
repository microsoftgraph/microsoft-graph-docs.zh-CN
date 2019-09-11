---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 218f3a4b1b03eedd9e9c8e99cd8c204304da976e
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2019
ms.locfileid: "36845953"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    ReceivedDateTime = DateTimeOffset.Parse("2016-10-19T10:37:00Z"),
    SentDateTime = DateTimeOffset.Parse("2016-10-19T10:37:00Z"),
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