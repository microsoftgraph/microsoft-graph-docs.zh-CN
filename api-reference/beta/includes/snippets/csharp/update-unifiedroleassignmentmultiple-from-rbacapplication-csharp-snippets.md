---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c3c8b1d60fd0cd45ed82c7d60a39eca2fd21fe3ebea43d188e1a176a6eb65b30
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220060"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignmentMultiple = new UnifiedRoleAssignmentMultiple
{
    PrincipalIds = new List<String>()
    {
        "0aeec2c1-fee7-4e02-b534-6f920d25b300",
        "2d5386a7-732f-44db-9cf8-f82dd2a1c0e0"
    }
};

await graphClient.RoleManagement.DeviceManagement.RoleAssignments["{unifiedRoleAssignmentMultiple-id}"]
    .Request()
    .UpdateAsync(unifiedRoleAssignmentMultiple);

```