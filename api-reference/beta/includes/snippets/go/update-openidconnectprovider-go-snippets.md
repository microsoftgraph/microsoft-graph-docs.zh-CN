---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d446fdebe3d89589fab0fc132cec30491704a128
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411957"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdentityProvider()
requestBody.SetAdditionalData(map[string]interface{}{
    "responseType": "id_token",
}
options := &msgraphsdk.IdentityProviderRequestBuilderPatchOptions{
    Body: requestBody,
}
identityProviderId := "identityProvider-id"
result, err := graphClient.IdentityProvidersById(&identityProviderId).Patch(options)


```