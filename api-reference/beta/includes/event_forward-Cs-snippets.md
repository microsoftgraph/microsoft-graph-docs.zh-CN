---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c90baf78633007b25810abc663b275d62045c60a
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34535901"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var toRecipients = new List<Recipient>()
{
    new Recipient
    {
        EmailAddress = new EmailAddress
        {
            Address = "danas@contoso.onmicrosoft.com",
            Name = "Dana Swope"
        }
    }
};

var comment = "Dana, hope you can make this meeting.";

await graphClient.Me.Events["{id}"]
    .Forward(comment,toRecipients)
    .Request()
    .PostAsync();

```