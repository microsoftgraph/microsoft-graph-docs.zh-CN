---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f347cb2d19a01f82cffd88d393355099122b69d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59061037"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignment = new UnifiedRoleAssignment
{
    RoleDefinitionId = "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    PrincipalId = "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
    DirectoryScopeId = "/"
};

await graphClient.RoleManagement.Directory.RoleAssignments
    .Request()
    .AddAsync(unifiedRoleAssignment);

```