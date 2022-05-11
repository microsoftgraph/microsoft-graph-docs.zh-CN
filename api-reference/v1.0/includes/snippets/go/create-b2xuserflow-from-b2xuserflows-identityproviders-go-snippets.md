---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cdb435b0321cb7f9359f25f8843277dfcc5d1377
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326511"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewB2xIdentityUserFlow()
id := "Partner"
requestBody.SetId(&id)
userFlowType := "signUpOrSignIn"
requestBody.SetUserFlowType(&userFlowType)
userFlowTypeVersion := float32(1)
requestBody.SetUserFlowTypeVersion(&userFlowTypeVersion)
requestBody.SetIdentityProviders( []IdentityProvider {
    msgraphsdk.NewIdentityProvider(),
    SetAdditionalData(map[string]interface{}{
        "id": "Facebook-OAuth",
        "type": "Facebook",
        "name": "Facebook",
    }
}
result, err := graphClient.Identity().B2xUserFlows().Post(requestBody)


```