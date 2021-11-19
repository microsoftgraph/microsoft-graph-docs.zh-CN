---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86216f58628016125e5fd6ac38351a5e9d4dc4bc
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083729"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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