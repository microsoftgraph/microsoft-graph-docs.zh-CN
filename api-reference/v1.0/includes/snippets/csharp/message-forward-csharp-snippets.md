---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52493263cd79921e38079789a0c788cd3a6981216e155fab17f18e9ceae8ac0a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162968"
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

await graphClient.Me.Messages["{message-id}"]
    .Forward(toRecipients,null,comment)
    .Request()
    .PostAsync();

```