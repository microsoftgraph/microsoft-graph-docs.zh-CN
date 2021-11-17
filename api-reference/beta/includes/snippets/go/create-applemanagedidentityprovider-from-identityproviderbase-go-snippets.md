---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: acb7b56a1abb59abf814af9bda92ca66f09ddd6d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61015101"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewIdentityProviderBase()
displayName := "Sign in with Apple"
requestBody.SetDisplayName(&displayName)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.appleManagedIdentityProvider",
    "developerId": "UBF8T346G9",
    "serviceId": "com.microsoft.rts.b2c.test.client",
    "keyId": "99P6D879C4",
    "certificateData": "******",
}
options := &msgraphsdk.IdentityProvidersRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Identity().IdentityProviders().Post(options)


```