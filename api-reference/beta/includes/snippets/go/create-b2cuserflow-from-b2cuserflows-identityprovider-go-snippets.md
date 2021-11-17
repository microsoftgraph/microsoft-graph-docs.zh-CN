---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2145acf158063a288cbf3c8541cf4d42b6cbc7d4
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60998150"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
options := &msgraphsdk.B2cUserFlowsRequestBuilderPostOptions{
    Body: requestBody,
    H: headers,
}
result, err := graphClient.Identity().B2cUserFlows().Post(options)


```