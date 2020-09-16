---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dcfbf4de2104acca2e1efe7c31f5f32408d93556
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47842867"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authorizationPolicy = new AuthorizationPolicy
{
    BlockMsolPowerShell = true
};

await graphClient.Policies.AuthorizationPolicy["authorizationPolicy"]
    .Request()
    .UpdateAsync(authorizationPolicy);

```