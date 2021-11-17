---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b85577fe0c0530ded863d43c20eb67852a5de6f7
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61030456"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewContinuousAccessEvaluationPolicy()
migrate := true
requestBody.SetMigrate(&migrate)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.continuousAccessEvaluationPolicy",
}
options := &msgraphsdk.ContinuousAccessEvaluationPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
graphClient.Identity().ContinuousAccessEvaluationPolicy().Patch(options)


```