---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e8f4d943849ac75094e9f19675f57bd9b4d720cb
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44794462"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignment = new UnifiedRoleAssignment
{
    RoleDefinitionId = "fe930be7-5e62-47db-91af-98c3a49a38b1",
    PrincipalId = "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
    DirectoryScopeId = "/administrativeUnits/5d107bba-d8e2-4e13-b6ae-884be90e5d1a"
};

await graphClient.RoleManagement.Directory.RoleAssignments
    .Request()
    .AddAsync(unifiedRoleAssignment);

```