---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17adf2f7ac7f22c67b6babbf8720aab452b50f1f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097192"
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
graphClient.Policies().FeatureRolloutPoliciesById(&featureRolloutPolicyId).Patch(options)


```