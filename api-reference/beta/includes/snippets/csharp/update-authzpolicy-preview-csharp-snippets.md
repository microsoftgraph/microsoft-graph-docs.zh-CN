---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f34a1bc7a0f5b0db924e4060631cdfbedf00802cab83545f6e1b9710ab88baa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903161"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authorizationPolicy = new AuthorizationPolicy
{
    EnabledPreviewFeatures = new List<String>()
    {
        "assignGroupsToRoles"
    }
};

await graphClient.Policies.AuthorizationPolicy["{authorizationPolicy-id}"]
    .Request()
    .UpdateAsync(authorizationPolicy);

```