---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 562d1fc6e3fee60b57ce208276a11328b14a70cd6e50f5b0137e1ec84bbc4ef4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277735"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignmentMultiple = new UnifiedRoleAssignmentMultiple
{
    DisplayName = "NewName",
    Description = "A new roleAssignment"
};

await graphClient.RoleManagement.CloudPC.RoleAssignments["{unifiedRoleAssignmentMultiple-id}"]
    .Request()
    .UpdateAsync(unifiedRoleAssignmentMultiple);

```