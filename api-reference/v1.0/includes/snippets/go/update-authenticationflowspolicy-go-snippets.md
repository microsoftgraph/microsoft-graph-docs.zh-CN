---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c463cf28b61353fbaf885ae5e6028e2309925d26
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087187"
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
graphClient.Policies().AuthenticationFlowsPolicy().Patch(options)


```