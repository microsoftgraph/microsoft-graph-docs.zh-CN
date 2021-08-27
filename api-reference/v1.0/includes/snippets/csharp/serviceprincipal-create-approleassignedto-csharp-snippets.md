---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f8266efa8b7da11aaeb91ea2f118b36680eabe617111cf537e92b9c5c89cc75
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902949"
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