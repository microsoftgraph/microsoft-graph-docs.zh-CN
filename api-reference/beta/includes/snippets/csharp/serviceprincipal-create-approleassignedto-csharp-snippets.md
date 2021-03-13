---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44638ca3d75ccf206d692b4d5fca4fc24e2b6083
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801313"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignment = new AppRoleAssignment
{
    PrincipalId = Guid.Parse("33ad69f9-da99-4bed-acd0-3f24235cb296"),
    ResourceId = Guid.Parse("9028d19c-26a9-4809-8e3f-20ff73e2d75e"),
    AppRoleId = Guid.Parse("ef7437e6-4f94-4a0a-a110-a439eb2aa8f7")
};

await graphClient.ServicePrincipals["{servicePrincipal-id}"].AppRoleAssignedTo
    .Request()
    .AddAsync(appRoleAssignment);

```