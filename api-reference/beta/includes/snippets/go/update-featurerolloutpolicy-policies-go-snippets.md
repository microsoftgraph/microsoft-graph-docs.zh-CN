---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4624356c6a21cc5f97e211fce69fdb104449df59
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412256"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewFeatureRolloutPolicy()
displayName := "PasswordHashSync Rollout Policy"
requestBody.SetDisplayName(&displayName)
description := "PasswordHashSync Rollout Policy"
requestBody.SetDescription(&description)
isEnabled := true
requestBody.SetIsEnabled(&isEnabled)
isAppliedToOrganization := false
requestBody.SetIsAppliedToOrganization(&isAppliedToOrganization)
options := &msgraphsdk.FeatureRolloutPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
featureRolloutPolicyId := "featureRolloutPolicy-id"
result, err := graphClient.Policies().FeatureRolloutPoliciesById(&featureRolloutPolicyId).Patch(options)


```