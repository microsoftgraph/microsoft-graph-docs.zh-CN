---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ffbe95a8fb83dd2d0f8212e07e849cfdf7b00d4e
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458650"
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