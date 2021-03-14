---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1fa4fbbd279807d62060f6da0a3ad5a4dea5747
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803322"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignment = new AppRoleAssignment
{
    PrincipalId = Guid.Parse("8fce32da-1246-437b-99cd-76d1d4677bd5"),
    ResourceId = Guid.Parse("9028d19c-26a9-4809-8e3f-20ff73e2d75e"),
    AppRoleId = Guid.Parse("ef7437e6-4f94-4a0a-a110-a439eb2aa8f7")
};

await graphClient.ServicePrincipals["{servicePrincipal-id}"].AppRoleAssignments
    .Request()
    .AddAsync(appRoleAssignment);

```