---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5103864baa63537e03f3d85431cf9b1740563c12
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34452847"
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

await graphClient.Groups["{id}"].Threads["{id}"].Posts["{id}"]
    .Forward(comment,toRecipients)
    .Request()
    .PostAsync();

```