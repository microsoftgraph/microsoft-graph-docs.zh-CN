---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7306eae387fd2ad75305ea7888cf6cd1e5e2a2f788fc99695b902bcb08c05514
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903157"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authorizationPolicy = new AuthorizationPolicy
{
    PermissionGrantPolicyIdsAssignedToDefaultUserRole = new List<String>()
    {
    }
};

await graphClient.Policies.AuthorizationPolicy["{authorizationPolicy-id}"]
    .Request()
    .UpdateAsync(authorizationPolicy);

```