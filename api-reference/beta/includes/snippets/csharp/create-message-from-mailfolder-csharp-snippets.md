---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e69b68dd539a4aeb3b6f3e944b5c9946eeaa33d48bdfd481e648c304e4a617a5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221327"
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

await graphClient.Me.MailFolders["{mailFolder-id}"].Messages
    .Request()
    .AddAsync(message);

```