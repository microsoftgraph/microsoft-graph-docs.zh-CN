---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16342fb10eae41f29123d81ba01c716d651e7bc7
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326445"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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
scheduleSettings := msgraphsdk.NewAccessReviewHistoryScheduleSettings()
requestBody.SetScheduleSettings(scheduleSettings)
reportRange := "P1M"
scheduleSettings.SetReportRange(&reportRange)
recurrence := msgraphsdk.NewPatternedRecurrence()
scheduleSettings.SetRecurrence(recurrence)
pattern := msgraphsdk.NewRecurrencePattern()
recurrence.SetPattern(pattern)
type := "monthly"
pattern.SetType(&type)
interval := int32(1)
pattern.SetInterval(&interval)
range := msgraphsdk.NewRecurrenceRange()
recurrence.SetRange(range)
type := "noEnd"
range.SetType(&type)
startDate := "2018-08-03T21:02:30.667Z"
range.SetStartDate(&startDate)
range.SetAdditionalData(map[string]interface{}{
    "count": ,
}
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
result, err := graphClient.IdentityGovernance().AccessReviews().HistoryDefinitions().Post(requestBody)


```