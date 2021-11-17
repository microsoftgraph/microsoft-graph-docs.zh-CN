---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 193c678cf0491a6ee431213e91c69622d7a82f39
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60987907"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewAccessReviewHistoryDefinition()
displayName := "Last quarter's group reviews April 2021"
requestBody.SetDisplayName(&displayName)
requestBody.SetDecisions( []AccessReviewHistoryDecisionFilter {
    "approve",
    "deny",
    "dontKnow",
    "notReviewed",
    "notNotified",
}
reviewHistoryPeriodStartDateTime, err := time.Parse(time.RFC3339, "2021-01-01T00:00:00Z")
requestBody.SetReviewHistoryPeriodStartDateTime(&reviewHistoryPeriodStartDateTime)
reviewHistoryPeriodEndDateTime, err := time.Parse(time.RFC3339, "2021-04-05T00:00:00Z")
requestBody.SetReviewHistoryPeriodEndDateTime(&reviewHistoryPeriodEndDateTime)
requestBody.SetScopes( []AccessReviewScope {
    msgraphsdk.NewAccessReviewScope(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
        "queryType": "MicrosoftGraph",
        "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')",
        "queryRoot": nil,
    }
    msgraphsdk.NewAccessReviewScope(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
        "queryType": "MicrosoftGraph",
        "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')",
        "queryRoot": nil,
    }
}
options := &msgraphsdk.HistoryDefinitionsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.IdentityGovernance().AccessReviews().HistoryDefinitions().Post(options)


```