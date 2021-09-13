---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b132249eae78e613f02a3ff4ea7a955adbc72b7a98bee708ce952b356865183
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277508"
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