---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35c5dea5a7b6b2bfa2467ce9ea32b11be0290d32
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412182"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAuthenticationFlowsPolicy()
selfServiceSignUp := msgraphsdk.NewSelfServiceSignUpAuthenticationFlowConfiguration()
requestBody.SetSelfServiceSignUp(selfServiceSignUp)
isEnabled := true
selfServiceSignUp.SetIsEnabled(&isEnabled)
options := &msgraphsdk.AuthenticationFlowsPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
result, err := graphClient.Policies().AuthenticationFlowsPolicy().Patch(options)


```