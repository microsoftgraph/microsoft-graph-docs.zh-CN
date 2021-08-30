---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5cc2df617f3cd1e7f9529fce2e09e7eb743e1c55d45b2f8ccd41523f84561195
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216010"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignment = new AppRoleAssignment
{
    PrincipalId = Guid.Parse("9028d19c-26a9-4809-8e3f-20ff73e2d75e"),
    ResourceId = Guid.Parse("8fce32da-1246-437b-99cd-76d1d4677bd5"),
    AppRoleId = Guid.Parse("498476ce-e0fe-48b0-b801-37ba7e2685c6")
};

await graphClient.ServicePrincipals["{servicePrincipal-id}"].AppRoleAssignments
    .Request()
    .AddAsync(appRoleAssignment);

```