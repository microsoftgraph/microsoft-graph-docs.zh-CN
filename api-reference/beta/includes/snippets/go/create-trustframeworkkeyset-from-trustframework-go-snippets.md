---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37dd17ce9b0b47522660a18a7c2e6ae2287c84b0
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088451"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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