---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 40486e6011860d118f599534d211612b50fc32514a3172620fb825cb397740f4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904226"
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