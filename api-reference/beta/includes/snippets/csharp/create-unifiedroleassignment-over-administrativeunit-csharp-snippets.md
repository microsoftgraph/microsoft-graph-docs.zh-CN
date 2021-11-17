---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5193c5365468a9887b82954a412c94ff566852028eb74a5e86163778cf685549
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904224"
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