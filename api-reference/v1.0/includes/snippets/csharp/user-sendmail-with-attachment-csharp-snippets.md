---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e986e9ca6780adef83e0ac5a13dc9e8264405ac
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684379"
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
    Attachments = (IMessageAttachmentsCollectionPage)new List<Attachment>()
    {
        new FileAttachment
        {
            Name = "attachment.txt",
            ContentType = "text/plain",
            ContentBytes = Encoding.ASCII.GetBytes("SGVsbG8gV29ybGQh")
        }
    }
};

await graphClient.Me
    .SendMail(message,null)
    .Request()
    .PostAsync();

```