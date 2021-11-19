---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e5356c6096d11a72194d2416fa548121c169ad0
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100032"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewFeatureRolloutPolicy()
displayName := "PassthroughAuthentication rollout policy"
requestBody.SetDisplayName(&displayName)
description := "PassthroughAuthentication rollout policy"
requestBody.SetDescription(&description)
feature := "passthroughAuthentication"
requestBody.SetFeature(&feature)
isEnabled := true
requestBody.SetIsEnabled(&isEnabled)
isAppliedToOrganization := false
requestBody.SetIsAppliedToOrganization(&isAppliedToOrganization)
options := &msgraphsdk.FeatureRolloutPoliciesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Policies().FeatureRolloutPolicies().Post(options)


```