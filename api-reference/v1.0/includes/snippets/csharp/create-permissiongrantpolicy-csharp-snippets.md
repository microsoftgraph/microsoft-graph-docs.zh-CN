---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ffbe95a8fb83dd2d0f8212e07e849cfdf7b00d4e
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524115"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissionGrantPolicy = new PermissionGrantPolicy
{
    Id = "my-custom-consent-policy",
    DisplayName = "Custom application consent policy",
    Description = "A custom permission grant policy to customize conditions for granting consent."
};

await graphClient.Policies.PermissionGrantPolicies
    .Request()
    .AddAsync(permissionGrantPolicy);

```