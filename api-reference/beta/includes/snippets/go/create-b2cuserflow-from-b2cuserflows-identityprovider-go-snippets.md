---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 05cffe8a1a6298b1f92c322892d1b28ccb93245b
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328718"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewB2cIdentityUserFlow()
id := "Customer"
requestBody.SetId(&id)
userFlowType := "signUpOrSignIn"
requestBody.SetUserFlowType(&userFlowType)
userFlowTypeVersion := float32(3)
requestBody.SetUserFlowTypeVersion(&userFlowTypeVersion)
requestBody.SetIdentityProviders( []IdentityProvider {
    msgraphsdk.NewIdentityProvider(),
    SetAdditionalData(map[string]interface{}{
        "id": "Facebook-OAuth",
    }
}
headers := map[string]string{
    "Location": "https://graph.microsoft.com/beta/identity/b2cUserFlows('B2C_1_Customer')"
}
options := &msgraphsdk.B2cUserFlowsRequestBuilderPostRequestConfiguration{
    Headers: headers,
}
result, err := graphClient.Identity().B2cUserFlows().PostWithRequestConfigurationAndResponseHandler(requestBody, options, nil)


```