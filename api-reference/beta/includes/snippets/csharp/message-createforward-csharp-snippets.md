---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e7a08195b3aa697d09bd0bcd90b49e721b21b47bf9b71378cb77eff906445df7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104776"
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

await graphClient.Me.Messages["{message-id}"]
    .CreateForward(null,message,comment)
    .Request()
    .PostAsync();

```