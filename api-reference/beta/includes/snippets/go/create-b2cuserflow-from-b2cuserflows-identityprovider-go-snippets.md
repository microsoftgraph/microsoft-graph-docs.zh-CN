---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bcd92eede81b7fecaf7e44685b445469f43e628f
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098789"
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
id := "Facebook-OAuth"
    SetId(&id)
}
headers := map[string]string{
    "Location": "https://graph.microsoft.com/beta/identity/b2cUserFlows('B2C_1_Customer')"
}
options := &msgraphsdk.B2cUserFlowsRequestBuilderPostRequestConfiguration{
    Headers: headers,
}
result, err := graphClient.Identity().B2cUserFlows().PostWithRequestConfigurationAndResponseHandler(requestBody, options, nil)


```