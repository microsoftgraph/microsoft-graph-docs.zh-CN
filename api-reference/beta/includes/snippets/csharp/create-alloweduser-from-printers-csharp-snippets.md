---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3762667dd24c365c4666d1e458e5757a6840a1ee
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947802"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printUserIdentity = new PrintUserIdentity
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id","https://graph.microsoft.com/beta/users/{id}"}
    }
};

await graphClient.Print.Printers["{id}"].AllowedUsers.References
    .Request()
    .AddAsync(printUserIdentity);

```