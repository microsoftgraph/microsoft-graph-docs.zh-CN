---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22a2ef8c3a3a9d7a45c2f2d26b0cb8afa64a2359
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805857"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissionGrantPolicy = new PermissionGrantPolicy
{
    DisplayName = "Custom permission grant policy"
};

await graphClient.Policies.PermissionGrantPolicies["{permissionGrantPolicy-id}"]
    .Request()
    .UpdateAsync(permissionGrantPolicy);

```