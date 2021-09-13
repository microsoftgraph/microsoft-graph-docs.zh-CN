---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7232b109e972d83000687d9a7bf9dfeb4ab13cbab98b3b2f09311e2b44041050
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903530"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignment = new AppRoleAssignment
{
    PrincipalId = Guid.Parse("7679d9a4-2323-44cd-b5c2-673ec88d8b12"),
    ResourceId = Guid.Parse("076e8b57-bac8-49d7-9396-e3449b685055"),
    AppRoleId = Guid.Parse("00000000-0000-0000-0000-000000000000")
};

await graphClient.Groups["{group-id}"].AppRoleAssignments
    .Request()
    .AddAsync(appRoleAssignment);

```