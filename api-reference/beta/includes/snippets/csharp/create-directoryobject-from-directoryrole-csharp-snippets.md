---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b3c009a4a63e75a4058c41898f6c416a1d763c3
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681059"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"directoryObject", "{}"}
    }
};

await graphClient.DirectoryRoles["{id}"].Members.References
    .Request()
    .AddAsync(directoryObject);

```