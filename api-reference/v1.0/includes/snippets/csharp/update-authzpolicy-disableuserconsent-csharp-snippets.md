---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e8a46b8eb08960a14269fb666d83e8001afa4910
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691371"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authorizationPolicy = new AuthorizationPolicy
{
    DefaultUserRolePermissions = new DefaultUserRolePermissions
    {
        PermissionGrantPoliciesAssigned = new List<String>()
        {
        }
    }
};

await graphClient.Policies.AuthorizationPolicy
    .Request()
    .UpdateAsync(authorizationPolicy);

```