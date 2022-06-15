---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 700da3e5b249ff79bf457b0b36e5966217e7485b
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098741"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessReviewInstance()
scope := msgraphsdk.NewAccessReviewScope()
requestBody.SetScope(scope)
scope.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
    "principalScopes":  []Object {
    }
    "resourceScopes":  []Object {
    }
}
requestBody.SetReviewers( []AccessReviewReviewerScope {
    msgraphsdk.NewAccessReviewReviewerScope(),
query := "/users/1ed8ac56-4827-4733-8f80-86adc2e67db5"
    SetQuery(&query)
queryType := "MicrosoftGraph"
    SetQueryType(&queryType)
}
requestBody.SetFallbackReviewers( []AccessReviewReviewerScope {
    msgraphsdk.NewAccessReviewReviewerScope(),
query := "/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e"
    SetQuery(&query)
queryType := "MicrosoftGraph"
    SetQueryType(&queryType)
    msgraphsdk.NewAccessReviewReviewerScope(),
query := "/users/1ed8ac56-4827-4733-8f80-86adc2e67db5"
    SetQuery(&query)
queryType := "MicrosoftGraph"
    SetQueryType(&queryType)
}
accessReviewScheduleDefinitionId := "accessReviewScheduleDefinition-id"
accessReviewInstanceId := "accessReviewInstance-id"
graphClient.IdentityGovernance().AccessReviews().DefinitionsById(&accessReviewScheduleDefinitionId).InstancesById(&accessReviewInstanceId).Patch(requestBody)


```