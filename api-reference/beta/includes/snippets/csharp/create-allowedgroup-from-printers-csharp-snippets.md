---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 225439b3a3e0d54cef4a9bc01129ef4d67a355b8
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947829"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printIdentity = new PrintIdentity
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id","https://graph.microsoft.com/beta/groups/{id}"}
    }
};

await graphClient.Print.Printers["{id}"].AllowedGroups.References
    .Request()
    .AddAsync(printIdentity);

```