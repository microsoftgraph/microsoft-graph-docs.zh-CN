---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8e1ef2af7a58386f36f4233796be08590968a384
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34475421"
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