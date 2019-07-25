---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8e1ef2af7a58386f36f4233796be08590968a384
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725289"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignment = new AppRoleAssignment
{
    CreationTimestamp = "2016-10-19T10:37:00Z",
    PrincipalDisplayName = "principalDisplayName-value",
    PrincipalId = "principalId-value",
    PrincipalType = "principalType-value",
    ResourceDisplayName = "resourceDisplayName-value"
};

await graphClient.ServicePrincipals["{id}"].AppRoleAssignments
    .Request()
    .AddAsync(appRoleAssignment);

```