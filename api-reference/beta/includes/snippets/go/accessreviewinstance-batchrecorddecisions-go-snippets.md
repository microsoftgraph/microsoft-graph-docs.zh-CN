---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75d098fe5ca4037e1527e7294897b27e0c2151ae
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412100"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
decision := "Approve"
requestBody.SetDecision(&decision)
justification := "All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team"
requestBody.SetJustification(&justification)
resourceId := "a5c51e59-3fcd-4a37-87a1-835c0c21488a"
requestBody.SetResourceId(&resourceId)
options := &msgraphsdk.BatchRecordDecisionsRequestBuilderPostOptions{
    Body: requestBody,
}
accessReviewInstanceId := "accessReviewInstance-id"
graphClient.Me().PendingAccessReviewInstancesById(&accessReviewInstanceId).BatchRecordDecisions(accessReviewInstance-id).Post(options)


```