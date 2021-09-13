---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbfa44736e13600d7da318502cac2a9a205c691482950aa63abe7b0d70e2509e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158327"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignment = new AppRoleAssignment
{
    PrincipalId = Guid.Parse("cde330e5-2150-4c11-9c5b-14bfdc948c79"),
    ResourceId = Guid.Parse("8e881353-1735-45af-af21-ee1344582a4d"),
    AppRoleId = Guid.Parse("00000000-0000-0000-0000-000000000000")
};

await graphClient.Users["{user-id}"].AppRoleAssignments
    .Request()
    .AddAsync(appRoleAssignment);

```