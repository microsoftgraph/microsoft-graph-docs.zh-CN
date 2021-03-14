---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 66503fceb166d8ab98ca5dbea2fd6963d9ffbcac
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798940"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignment = new AppRoleAssignment
{
    PrincipalId = Guid.Parse("principalId-value"),
    ResourceId = Guid.Parse("resourceId-value"),
    AppRoleId = Guid.Parse("appRoleId-value")
};

await graphClient.Users["{user-id}"].AppRoleAssignments
    .Request()
    .AddAsync(appRoleAssignment);

```