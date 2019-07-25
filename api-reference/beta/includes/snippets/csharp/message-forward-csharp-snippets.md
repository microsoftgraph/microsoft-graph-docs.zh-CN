---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 776f5a32ec169863087a2d7c897a5f561c27db63
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729735"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    IsDeliveryReceiptRequested = true,
    ToRecipients = new List<Recipient>()
    {
        new Recipient
        {
            EmailAddress = new EmailAddress
            {
                Address = "danas@contoso.onmicrosoft.com",
                Name = "Dana Swope"
            }
        }
    }
};

var comment = "Dana, just want to make sure you get this.";

await graphClient.Me.Messages["AAMkADA1MTAAAH5JaLAAA="]
    .Forward(message,comment,toRecipients)
    .Request()
    .PostAsync();

```