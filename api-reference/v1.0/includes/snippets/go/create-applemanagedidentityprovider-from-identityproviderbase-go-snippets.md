---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2487f5afe7b0a9c0a89ca4e020ca2d7563359522
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085211"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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