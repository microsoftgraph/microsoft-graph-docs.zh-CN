---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2cc9e7594b273044a97236293ecafe6fd28e2982
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808924"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    ReceivedDateTime = DateTimeOffset.Parse("datetime-value"),
    SentDateTime = DateTimeOffset.Parse("datetime-value"),
    HasAttachments = true,
    Subject = "subject-value",
    Body = new ItemBody
    {
        ContentType = BodyType.Text,
        Content = "content-value"
    },
    BodyPreview = "bodyPreview-value"
};

await graphClient.Me.MailFolders["{mailFolder-id}"].Messages
    .Request()
    .AddAsync(message);

```