---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0cdf3db51e1fe7dbc4849ba36826c2b981917b73
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337649"
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
options := &msgraphsdk.HistoryDefinitionsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.IdentityGovernance().AccessReviews().HistoryDefinitions().Post(options)


```