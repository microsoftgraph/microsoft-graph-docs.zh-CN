---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 27a9dc3dcf2d16ed26b8a05c88dcd0533f30c979
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443955"
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

var comment = "Samantha, Randi, would you name the group please?";

await graphClient.Me.Messages["AAMkADA1MTAAAAqldOAAA="]
    .Reply(message,comment)
    .Request()
    .PostAsync();

```