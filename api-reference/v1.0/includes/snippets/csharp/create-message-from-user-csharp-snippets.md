---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e826eef104b1b63c40f7552f2a944e09352ac946
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608022"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    Subject = "Did you see last night's game?",
    Importance = Importance.Low,
    Body = new ItemBody
    {
        ContentType = BodyType.Html,
        Content = "They were <b>awesome</b>!"
    },
    ToRecipients = new List<Recipient>()
    {
        new Recipient
        {
            EmailAddress = new EmailAddress
            {
                Address = "AdeleV@contoso.onmicrosoft.com"
            }
        }
    }
};

await graphClient.Me.Messages
    .Request()
    .AddAsync(message);

```