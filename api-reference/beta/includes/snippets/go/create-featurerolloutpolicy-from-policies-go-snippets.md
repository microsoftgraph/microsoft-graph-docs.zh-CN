---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a955c8e2bacae3d90730e069ae88bbd1b0e023de
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326569"
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
result, err := graphClient.Policies().FeatureRolloutPolicies().Post(requestBody)


```