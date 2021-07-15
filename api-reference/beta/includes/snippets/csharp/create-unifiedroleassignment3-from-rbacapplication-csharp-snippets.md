---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eaf8ff2f99249b6b85ee644f430ba355dcff5636
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442190"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignment = new UnifiedRoleAssignment
{
    PrincipalId = "679a9213-c497-48a4-830a-8d3d25d94ddc",
    RoleDefinitionId = "ae79f266-94d4-4dab-b730-feca7e132178",
    AppScopeId = "/AccessPackageCatalog/beedadfe-01d5-4025-910b-84abb9369997"
};

await graphClient.RoleManagement.EntitlementManagement.RoleAssignments
    .Request()
    .AddAsync(unifiedRoleAssignment);

```