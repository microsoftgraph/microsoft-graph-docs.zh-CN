---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6e8ebcbe132839a9ce4497c36704b794ff8dabe3f729c9f903a04a7f6b0ec26
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333569"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenLifetimePolicy = new TokenLifetimePolicy
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/v1.0/policies/tokenLifetimePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"}
    }
};

await graphClient.Applications["{application-id}"].TokenLifetimePolicies.References
    .Request()
    .AddAsync(tokenLifetimePolicy);

```