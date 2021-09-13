---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1878bdba6ac814608514339d0b8c6ea6cb6c43ae0778cde110b16f7c0daebc9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332167"
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