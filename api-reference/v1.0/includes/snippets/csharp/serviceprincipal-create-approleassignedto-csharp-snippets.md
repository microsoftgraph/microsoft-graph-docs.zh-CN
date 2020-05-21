---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e50edb7230713802907ef7cfdbe8f9ed59311a5
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335053"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignment = new AppRoleAssignment
{
    PrincipalId = Guid.Parse("principalId-value"),
    ResourceId = Guid.Parse("resourceId-value"),
    AppRoleId = Guid.Parse("appRoleId-value")
};

await graphClient.ServicePrincipals["{id}"].AppRoleAssignedTo
    .Request()
    .AddAsync(appRoleAssignment);

```