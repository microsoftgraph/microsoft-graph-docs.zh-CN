---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 56a35e0a6fce5d0eeef1f4c19b07ce6d602ad643
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411964"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewContinuousAccessEvaluationPolicy()
migrate := true
requestBody.SetMigrate(&migrate)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.continuousAccessEvaluationPolicy",
}
options := &msgraphsdk.ContinuousAccessEvaluationPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
result, err := graphClient.Identity().ContinuousAccessEvaluationPolicy().Patch(options)


```