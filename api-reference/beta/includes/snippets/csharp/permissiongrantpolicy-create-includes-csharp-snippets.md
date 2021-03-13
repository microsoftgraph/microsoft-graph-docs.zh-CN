---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17fa0f854a47b8ea192089a2594c3811ac5d1ec8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807518"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissionGrantConditionSet = new PermissionGrantConditionSet
{
    PermissionType = PermissionType.Delegated,
    ClientApplicationsFromVerifiedPublisherOnly = true
};

await graphClient.Policies.PermissionGrantPolicies["{permissionGrantPolicy-id}"].Includes
    .Request()
    .AddAsync(permissionGrantConditionSet);

```