---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ac13d1c44ecc9918633e211ddeb32d126a37eeb
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458701"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissionGrantConditionSet = new PermissionGrantConditionSet
{
    PermissionType = PermissionType.Delegated,
    ResourceApplication = "00000003-0000-0000-c000-000000000000"
};

await graphClient.Policies.PermissionGrantPolicies["my-custom-consent-policy"].Excludes
    .Request()
    .AddAsync(permissionGrantConditionSet);

```