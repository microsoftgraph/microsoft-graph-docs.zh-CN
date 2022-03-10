---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e877a36b6ac901218e67d7fe4529f39b8b0c4f97
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412096"
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
    SetAdditionalData(map[string]interface{}{
        "query": "/users/1ed8ac56-4827-4733-8f80-86adc2e67db5",
        "queryType": "MicrosoftGraph",
    }
}
requestBody.SetFallbackReviewers( []AccessReviewReviewerScope {
    msgraphsdk.NewAccessReviewReviewerScope(),
    SetAdditionalData(map[string]interface{}{
        "query": "/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e",
        "queryType": "MicrosoftGraph",
    }
    msgraphsdk.NewAccessReviewReviewerScope(),
    SetAdditionalData(map[string]interface{}{
        "query": "/users/1ed8ac56-4827-4733-8f80-86adc2e67db5",
        "queryType": "MicrosoftGraph",
    }
}
options := &msgraphsdk.AccessReviewInstanceRequestBuilderPatchOptions{
    Body: requestBody,
}
accessReviewScheduleDefinitionId := "accessReviewScheduleDefinition-id"
accessReviewInstanceId := "accessReviewInstance-id"
result, err := graphClient.IdentityGovernance().AccessReviews().DefinitionsById(&accessReviewScheduleDefinitionId).InstancesById(&accessReviewInstanceId).Patch(options)


```