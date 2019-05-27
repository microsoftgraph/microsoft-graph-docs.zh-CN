---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 97b80561770acfde66f61a04ec266948ed29bc54
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439888"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleAssignment = new PrivilegedRoleAssignment
{
    UserId = "userId-value",
    RoleId = "roleId-value"
};

await graphClient.PrivilegedRoleAssignments
    .Request()
    .AddAsync(privilegedRoleAssignment);

```