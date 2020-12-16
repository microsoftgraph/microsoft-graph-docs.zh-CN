---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e2a38fa6fbc64da8b6948664814ee316fcf7416
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49692626"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = new User
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/beta/users/{id}"}
    }
};

await graphClient.Print.Shares["{id}"].AllowedUsers.References
    .Request()
    .AddAsync(user);

```