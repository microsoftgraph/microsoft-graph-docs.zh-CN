---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca817bccb8e08e78c5370349ed9df9fdc50bc473
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329181"
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
result, err := graphClient.Identity().IdentityProviders().Post(requestBody)


```