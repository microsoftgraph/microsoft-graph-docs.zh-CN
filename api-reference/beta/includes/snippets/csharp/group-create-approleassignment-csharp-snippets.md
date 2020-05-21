---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 56d609d9d0ebbc30eeb3c6e708be91d6406c3dbf
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332743"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignment = new AppRoleAssignment
{
    PrincipalId = Guid.Parse("principalId-value"),
    ResourceId = Guid.Parse("resourceId-value"),
    AppRoleId = Guid.Parse("appRoleId-value")
};

await graphClient.ServicePrincipals["{id}"].AppRoleAssignments
    .Request()
    .AddAsync(appRoleAssignment);

```