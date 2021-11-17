---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26ca4aeeedb9fa8741ec67f0bc17385f3225f16a584d02a14deb05f1b41f35a4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903156"
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