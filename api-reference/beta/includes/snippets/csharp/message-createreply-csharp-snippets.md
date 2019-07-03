---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 38f6164afc41be8f1724ca48fd2f8c6491edfb0f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521153"
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