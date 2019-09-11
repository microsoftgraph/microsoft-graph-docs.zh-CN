---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1af2e5fbd3ce1ef4fad9d9a1bc9802c19f4db024
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2019
ms.locfileid: "36845944"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignment = new AppRoleAssignment
{
    CreationTimestamp = DateTimeOffset.Parse("2016-10-19T10:37:00Z"),
    PrincipalDisplayName = "principalDisplayName-value",
    PrincipalId = Guid.Parse("principalId-value"),
    PrincipalType = "principalType-value",
    ResourceDisplayName = "resourceDisplayName-value"
};

await graphClient.ServicePrincipals["{id}"].AppRoleAssignments
    .Request()
    .AddAsync(appRoleAssignment);

```