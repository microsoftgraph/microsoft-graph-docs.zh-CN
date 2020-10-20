---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 38f6164afc41be8f1724ca48fd2f8c6491edfb0f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620072"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    ToRecipients = new List<Recipient>()
    {
        new Recipient
        {
            EmailAddress = new EmailAddress
            {
                Address = "samanthab@contoso.onmicrosoft.com",
                Name = "Samantha Booth"
            }
        },
        new Recipient
        {
            EmailAddress = new EmailAddress
            {
                Address = "randiw@contoso.onmicrosoft.com",
                Name = "Randi Welch"
            }
        }
    }
};

var comment = "Samantha, Randi, would you name the group if the project is approved, please?";

await graphClient.Me.Messages["AAMkADA1MTAAAAqldOAAA="]
    .CreateReply(message,comment)
    .Request()
    .PostAsync();

```