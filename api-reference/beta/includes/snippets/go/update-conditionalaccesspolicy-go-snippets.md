---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 669b5742c7773ed3490f1243ebe7b5a88b8bf2c5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62121238"
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
graphClient.Identity().ConditionalAccess().PoliciesById(&conditionalAccessPolicyId).Patch(options)


```