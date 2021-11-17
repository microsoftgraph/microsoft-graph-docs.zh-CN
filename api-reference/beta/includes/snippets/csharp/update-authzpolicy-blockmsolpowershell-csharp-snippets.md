---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ffa8a6b3217109b0decb73c10849bd0258e2190b02bcadb586249755124ac61
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903158"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authorizationPolicy = new AuthorizationPolicy
{
    BlockMsolPowerShell = true
};

await graphClient.Policies.AuthorizationPolicy["{authorizationPolicy-id}"]
    .Request()
    .UpdateAsync(authorizationPolicy);

```