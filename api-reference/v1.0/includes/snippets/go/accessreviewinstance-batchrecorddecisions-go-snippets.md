---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b306cd409264d185478821118ccf26216ca970ef
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60974732"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
accessReviewScheduleDefinitionId := "accessReviewScheduleDefinition-id"
accessReviewInstanceId := "accessReviewInstance-id"
graphClient.IdentityGovernance().AccessReviews().DefinitionsById(&accessReviewScheduleDefinitionId).InstancesById(&accessReviewInstanceId).BatchRecordDecisions().Post(options)


```