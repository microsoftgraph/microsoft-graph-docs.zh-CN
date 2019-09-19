---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4251c567a8395a213ef815176a72ddac7af07107
ms.sourcegitcommit: 997fbfe36b518e0a8c230ae2e62666bb5c829e7e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/19/2019
ms.locfileid: "37045329"
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

var comment = "Dana, just want to make sure you get this; you'll need this if the project gets approved.";

await graphClient.Me.Messages["AAMkADA1MTAAAH5JaLAAA="]
    .CreateForward(toRecipients,message,comment)
    .Request()
    .PostAsync();

```