---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ee62ecc04570fbbecda01da11ffce9b401811f13
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479842"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permission = new Permission
{
    Roles = new List<String>()
    {
        "read"
    }
};

await graphClient.Me.Drive.Items["{item-id}"].Permissions["{perm-id}"]
    .Request()
    .UpdateAsync(permission);

```