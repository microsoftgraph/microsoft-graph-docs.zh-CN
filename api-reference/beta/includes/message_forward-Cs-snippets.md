---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 776f5a32ec169863087a2d7c897a5f561c27db63
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444025"
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