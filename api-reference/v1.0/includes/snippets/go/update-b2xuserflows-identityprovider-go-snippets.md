---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a7e04f2ad8c20ff23a94df9bc60eb06cfec5be7
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411884"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/v1.0/identityProviders/Facebook-OAUTH",
}
options := &msgraphsdk.IdentityProviderRequestBuilderPostOptions{
    Body: requestBody,
}
b2xIdentityUserFlowId := "b2xIdentityUserFlow-id"
identityProviderId := "identityProvider-id"
graphClient.Identity().B2xUserFlowsById(&b2xIdentityUserFlowId).IdentityProvidersById(&identityProviderId).Post(options)


```