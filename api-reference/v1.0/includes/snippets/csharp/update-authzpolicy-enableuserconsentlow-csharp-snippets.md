---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8df0dc8ead8e887b861be74d37613a3d4e0f2916
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691368"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authorizationPolicy = new AuthorizationPolicy
{
    DefaultUserRolePermissions = new DefaultUserRolePermissions
    {
        PermissionGrantPoliciesAssigned = new List<String>()
        {
            "managePermissionGrantsForSelf.microsoft-user-default-low"
        }
    }
};

await graphClient.Policies.AuthorizationPolicy
    .Request()
    .UpdateAsync(authorizationPolicy);

```