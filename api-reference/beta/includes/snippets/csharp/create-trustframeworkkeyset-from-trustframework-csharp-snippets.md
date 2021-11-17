---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10277fba455bd222618dcf08c336a7532e65a2f72123b680a434e54df0c45ba2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279248"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var trustFrameworkKeySet = new TrustFrameworkKeySet
{
    Id = "keyset1",
    Keys = new List<TrustFrameworkKey>()
    {
        new TrustFrameworkKey
        {
            K = "k-value",
            X5c = new List<String>()
            {
                "x5c-value"
            },
            X5t = "x5t-value",
            Kty = "kty-value",
            Use = "use-value",
            Exp = 99,
            Nbf = 99,
            Kid = "kid-value",
            E = "e-value",
            N = "n-value",
            D = "d-value",
            P = "p-value",
            Q = "q-value",
            Dp = "dp-value",
            Dq = "dq-value",
            Qi = "qi-value"
        }
    }
};

await graphClient.TrustFramework.KeySets
    .Request()
    .AddAsync(trustFrameworkKeySet);

```