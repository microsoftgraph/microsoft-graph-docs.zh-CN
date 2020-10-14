---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5f29d2a090137e297c2b512d8eb99c403557c61
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458042"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2cAuthenticationMethodsPolicy = new B2cAuthenticationMethodsPolicy
{
    IsEmailPasswordAuthenticationEnabled = false,
    IsUserNameAuthenticationEnabled = true
};

await graphClient.Policies.B2cAuthenticationMethodsPolicy
    .Request()
    .UpdateAsync(b2cAuthenticationMethodsPolicy);

```