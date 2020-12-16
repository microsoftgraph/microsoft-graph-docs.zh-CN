---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 682ed62bde92e6a56b690ad80d02383f3b1510fd
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49692571"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = new Group
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/beta/groups/{id}"}
    }
};

await graphClient.Print.Shares["{id}"].AllowedGroups.References
    .Request()
    .AddAsync(group);

```