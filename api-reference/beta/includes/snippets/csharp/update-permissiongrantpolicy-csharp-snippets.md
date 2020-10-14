---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 088086278820f10df34f9a214e91240ccfb17b50
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48459608"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissionGrantPolicy = new PermissionGrantPolicy
{
    DisplayName = "Custom permission grant policy"
};

await graphClient.Policies.PermissionGrantPolicies["my-custom-consent-policy"]
    .Request()
    .UpdateAsync(permissionGrantPolicy);

```