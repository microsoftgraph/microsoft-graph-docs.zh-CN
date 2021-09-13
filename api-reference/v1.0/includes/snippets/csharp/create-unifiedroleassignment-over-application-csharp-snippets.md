---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a8bb419fe73fb8c06b2d12fa2c7c71da953ec51
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59061038"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignment = new UnifiedRoleAssignment
{
    PrincipalId = "6b937a9d-c731-465b-a844-2d5b5368c161",
    RoleDefinitionId = "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3",
    DirectoryScopeId = "/661e1310-bd76-4795-89a7-8f3c8f855bfc"
};

await graphClient.RoleManagement.Directory.RoleAssignments
    .Request()
    .AddAsync(unifiedRoleAssignment);

```