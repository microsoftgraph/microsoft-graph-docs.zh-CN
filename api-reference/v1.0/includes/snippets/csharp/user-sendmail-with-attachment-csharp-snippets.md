---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bea30b4b423136e7668996974bad0a0762ffa089
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774348"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    Subject = "Meet for lunch?",
    Body = new ItemBody
    {
        ContentType = BodyType.Text,
        Content = "The new cafeteria is open."
    },
    ToRecipients = new List<Recipient>()
    {
        new Recipient
        {
            EmailAddress = new EmailAddress
            {
                Address = "meganb@contoso.onmicrosoft.com"
            }
        }
    },
    Attachments = new List<Attachment>()
    {
        new FileAttachment
        {
            Name = "attachment.txt",
            ContentType = "text/plain",
            ContentBytes = "SGVsbG8gV29ybGQh"
        }
    }
};

await graphClient.Me
    .SendMail(message,null)
    .Request()
    .PostAsync();

```