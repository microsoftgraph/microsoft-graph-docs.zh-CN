---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e8f4d943849ac75094e9f19675f57bd9b4d720cb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59061030"
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