---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9cad8533a7adbf4f6efebe2a7aaef1587318fad9
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "37428845"
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

await graphClient.Me.Messages["{id}"]
    .Forward(toRecipients,null,comment)
    .Request()
    .PostAsync();

```