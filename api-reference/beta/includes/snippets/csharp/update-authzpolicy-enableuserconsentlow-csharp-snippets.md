---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f816239deba40ca3f263fdc4d5a38c6e108b8ee
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48457392"
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

await graphClient.Policies.AuthorizationPolicy["authorizationPolicy"]
    .Request()
    .UpdateAsync(authorizationPolicy);

```