---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8fa0d1b5d3bfc39f21f90fce8fa458dfc9487900
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181538"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignmentMultiple = new UnifiedRoleAssignmentMultiple
{
    RoleDefinitionId = "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    PrincipalIds = new List<String>()
    {
        "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
        "c1518aa9-4da5-4c84-a902-a31404023890"
    },
    DirectoryScopeIds = new List<String>()
    {
        "28ca5a85-489a-49a0-b555-0a6d81e56f0d",
        "8152656a-cf9a-4928-a457-1512d4cae295"
    }
};

await graphClient.RoleManagement.DeviceManagement.RoleAssignments
    .Request()
    .AddAsync(unifiedRoleAssignmentMultiple);

```