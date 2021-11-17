---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8eda353d6e3e0fe41ca24f95c1626496ee976af4
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61010428"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewTrustFrameworkKeySet()
id := "keyset1"
requestBody.SetId(&id)
requestBody.SetKeys( []TrustFrameworkKey {
    msgraphsdk.NewTrustFrameworkKey(),
    SetAdditionalData(map[string]interface{}{
        "k": "k-value",
        "x5c":  []String {
            "x5c-value",
        }
        "x5t": "x5t-value",
        "kty": "kty-value",
        "use": "use-value",
        "exp": ,
        "nbf": ,
        "kid": "kid-value",
        "e": "e-value",
        "n": "n-value",
        "d": "d-value",
        "p": "p-value",
        "q": "q-value",
        "dp": "dp-value",
        "dq": "dq-value",
        "qi": "qi-value",
    }
}
options := &msgraphsdk.KeySetsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.TrustFramework().KeySets().Post(options)


```