---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a4ed34678fc4bf89137b6a3bf628edb95f7939e
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47842846"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authorizationPolicy = new AuthorizationPolicy
{
    DefaultUserRolePermissions = new DefaultUserRolePermissions
    {
        AllowedToCreateApps = false
    }
};

await graphClient.Policies.AuthorizationPolicy["authorizationPolicy"]
    .Request()
    .UpdateAsync(authorizationPolicy);

```