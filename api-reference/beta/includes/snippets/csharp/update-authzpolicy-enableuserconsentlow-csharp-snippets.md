---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 649cdf29be1d5ac705a674a0c3de124d55d5daff
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786362"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authorizationPolicy = new AuthorizationPolicy
{
    PermissionGrantPolicyIdsAssignedToDefaultUserRole = new List<String>()
    {
        "managePermissionGrantsForSelf.microsoft-user-default-low"
    }
};

await graphClient.Policies.AuthorizationPolicy["{authorizationPolicy-id}"]
    .Request()
    .UpdateAsync(authorizationPolicy);

```