---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9826617a81adbacdc9aca0352c0c181d5bd59c014f16c485c401bad34b423191
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158453"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var trustFrameworkKeySet = new TrustFrameworkKeySet
{
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

await graphClient.TrustFramework.KeySets["{trustFrameworkKeySet-id}"]
    .Request()
    .PutAsync(trustFrameworkKeySet);

```