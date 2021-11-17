---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b9e59cd94f77e362a64b8feed5b00f469fa0e5cd
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60979850"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewAccessReviewInstanceDecisionItem()
decision := "Approve"
requestBody.SetDecision(&decision)
justification := "Kathleen still needs access to the Marketing group as she works in the Marketing organization."
requestBody.SetJustification(&justification)
options := &msgraphsdk.AccessReviewInstanceDecisionItemRequestBuilderPatchOptions{
    Body: requestBody,
}
accessReviewScheduleDefinitionId := "accessReviewScheduleDefinition-id"
accessReviewInstanceId := "accessReviewInstance-id"
accessReviewInstanceDecisionItemId := "accessReviewInstanceDecisionItem-id"
graphClient.IdentityGovernance().AccessReviews().DefinitionsById(&accessReviewScheduleDefinitionId).InstancesById(&accessReviewInstanceId).DecisionsById(&accessReviewInstanceDecisionItemId).Patch(options)


```