---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5758465726433e55a3f25145bfb3deeb2d4497d9
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691374"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authorizationPolicy = new AuthorizationPolicy
{
    BlockMsolPowerShell = true
};

await graphClient.Policies.AuthorizationPolicy
    .Request()
    .UpdateAsync(authorizationPolicy);

```