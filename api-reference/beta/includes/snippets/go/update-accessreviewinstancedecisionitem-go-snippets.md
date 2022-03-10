---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 150c19368c9fa380bf551e94774602bc6b30f051
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412095"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessReviewInstanceDecisionItem()
decision := "Approve"
requestBody.SetDecision(&decision)
justification := "This person is still on my team"
requestBody.SetJustification(&justification)
options := &msgraphsdk.AccessReviewInstanceDecisionItemRequestBuilderPatchOptions{
    Body: requestBody,
}
accessReviewScheduleDefinitionId := "accessReviewScheduleDefinition-id"
accessReviewInstanceId := "accessReviewInstance-id"
accessReviewStageId := "accessReviewStage-id"
accessReviewInstanceDecisionItemId := "accessReviewInstanceDecisionItem-id"
result, err := graphClient.IdentityGovernance().AccessReviews().DefinitionsById(&accessReviewScheduleDefinitionId).InstancesById(&accessReviewInstanceId).StagesById(&accessReviewStageId).DecisionsById(&accessReviewInstanceDecisionItemId).Patch(options)


```