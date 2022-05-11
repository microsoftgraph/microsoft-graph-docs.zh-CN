---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7fade0aecf28018e9bf5bd1fba293614a0cd13bd
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325759"
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
result, err := graphClient.TrustFramework().KeySets().Post(requestBody)


```