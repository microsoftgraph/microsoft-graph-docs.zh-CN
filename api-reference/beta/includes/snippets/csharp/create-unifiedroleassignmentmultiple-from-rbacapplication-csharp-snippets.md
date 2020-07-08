---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d39a4f49c84e05a4f5e277f7c02ca995a2229c46
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081716"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignmentMultiple = new UnifiedRoleAssignmentMultiple
{
    DisplayName = "My test role assignment 1",
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