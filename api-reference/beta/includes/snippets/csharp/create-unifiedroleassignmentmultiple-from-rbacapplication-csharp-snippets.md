---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88d8e7affeb3de73ac87ad9fe0a0ebd4e56a75d863b655c5da1abe4e1c69e534
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54275495"
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