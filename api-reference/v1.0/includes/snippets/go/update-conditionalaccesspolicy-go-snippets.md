---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e705da8dea0dd396a2ef645e60caa69435bd01f
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412601"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewConditionalAccessPolicy()
conditions := msgraphsdk.NewConditionalAccessConditionSet()
requestBody.SetConditions(conditions)
conditions.SetSignInRiskLevels( []RiskLevel {
    "high",
    "medium",
    "low",
}
options := &msgraphsdk.ConditionalAccessPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
conditionalAccessPolicyId := "conditionalAccessPolicy-id"
result, err := graphClient.Identity().ConditionalAccess().PoliciesById(&conditionalAccessPolicyId).Patch(options)


```