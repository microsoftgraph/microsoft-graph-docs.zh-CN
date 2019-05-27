---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 249ce76e9c70303b805ff8da5a3a7b0f9b2345a7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440217"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    Subject = "Party planning",
    ToRecipients = new List<Recipient>()
    {
        new Recipient
        {
            EmailAddress = new EmailAddress
            {
                Name = "Samantha Booth",
                Address = "samanthab@contoso.onmicrosoft.com"
            }
        }
    },
    Mentions = new List<Mention>()
    {
        new Mention
        {
            Mentioned = new EmailAddress
            {
                Name = "Dana Swope",
                Address = "danas@contoso.onmicrosoft.com"
            }
        }
    }
};

await graphClient.Me.Messages
    .Request()
    .AddAsync(message);

```