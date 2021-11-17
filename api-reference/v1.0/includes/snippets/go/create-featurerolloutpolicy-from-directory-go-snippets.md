---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 01cab8e5200fb1e1e054a6b5f2211c61466e6684
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60993165"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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