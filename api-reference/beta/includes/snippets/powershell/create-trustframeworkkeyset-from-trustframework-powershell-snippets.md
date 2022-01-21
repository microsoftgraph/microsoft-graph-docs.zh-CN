---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad0771d8629b928d7ad459a7115d281b6b0d9219
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62115309"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    Id = "keyset1"
    Keys = @(
        @{
            K = "k-value"
            X5c = @(
                "x5c-value"
            )
            X5t = "x5t-value"
            Kty = "kty-value"
            Use = "use-value"
            Exp = 99
            Nbf = 99
            Kid = "kid-value"
            E = "e-value"
            N = "n-value"
            D = "d-value"
            P = "p-value"
            Q = "q-value"
            Dp = "dp-value"
            Dq = "dq-value"
            Qi = "qi-value"
        }
    )
}

New-MgTrustFrameworkKeySet -BodyParameter $params

```