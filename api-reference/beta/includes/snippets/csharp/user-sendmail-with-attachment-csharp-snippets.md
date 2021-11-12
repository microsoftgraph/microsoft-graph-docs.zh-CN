---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a91e38a32bb619b8ca4530afa7fef1e1d04ee972ae40269dd1a1049b7f9e780c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277728"
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
    Attachments = new MessageAttachmentsCollectionPage()
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