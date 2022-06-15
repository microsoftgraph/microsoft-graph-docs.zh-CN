---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c117bd71e345deb1a58c400d3b33423e6c3c9c3
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098763"
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
id := "Facebook-OAuth"
    SetId(&id)
type := "Facebook"
    SetType(&type)
name := "Facebook"
    SetName(&name)
}
result, err := graphClient.Identity().B2xUserFlows().Post(requestBody)


```