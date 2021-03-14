---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b96bd138f8bd10d791878e065db1d83c387ed5d7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800292"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "comment-value";

var toRecipients = new List<Recipient>()
{
    new Recipient
    {
        EmailAddress = new EmailAddress
        {
            Name = "name-value",
            Address = "address-value"
        }
    }
};

await graphClient.Groups["{group-id}"].Threads["{conversationThread-id}"].Posts["{post-id}"]
    .Forward(toRecipients,comment)
    .Request()
    .PostAsync();

```