---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18fc3a09680cc5d7a15b20252833f660965d4c71
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326152"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessReviewScheduleDefinition()
displayName := "Group Multi-stage Access Review"
requestBody.SetDisplayName(&displayName)
descriptionForAdmins := "New scheduled access review"
requestBody.SetDescriptionForAdmins(&descriptionForAdmins)
descriptionForReviewers := "If you have any questions, contact jerry@contoso.com"
requestBody.SetDescriptionForReviewers(&descriptionForReviewers)
scope := msgraphsdk.NewAccessReviewScope()
requestBody.SetScope(scope)
scope.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups/02f3bafb-448c-487c-88c2-5fd65ce49a41/transitiveMembers",
    "queryType": "MicrosoftGraph",
}
requestBody.SetStageSettings( []AccessReviewStageSettings {
    msgraphsdk.NewAccessReviewStageSettings(),
    SetAdditionalData(map[string]interface{}{
        "stageId": "1",
        "durationInDays": ,
        "recommendationsEnabled": false,
        "decisionsThatWillMoveToNextStage":  []String {
            "NotReviewed",
            "Approve",
        }
        "reviewers":  []Object {
        }
    }
    msgraphsdk.NewAccessReviewStageSettings(),
    SetAdditionalData(map[string]interface{}{
        "stageId": "2",
        "dependsOn":  []String {
            "1",
        }
        "durationInDays": ,
        "recommendationsEnabled": true,
        "reviewers":  []Object {
        }
        "fallbackReviewers":  []Object {
        }
    }
}
settings := msgraphsdk.NewAccessReviewScheduleSettings()
requestBody.SetSettings(settings)
mailNotificationsEnabled := true
settings.SetMailNotificationsEnabled(&mailNotificationsEnabled)
reminderNotificationsEnabled := true
settings.SetReminderNotificationsEnabled(&reminderNotificationsEnabled)
justificationRequiredOnApproval := true
settings.SetJustificationRequiredOnApproval(&justificationRequiredOnApproval)
defaultDecisionEnabled := false
settings.SetDefaultDecisionEnabled(&defaultDecisionEnabled)
defaultDecision := "None"
settings.SetDefaultDecision(&defaultDecision)
instanceDurationInDays := int32(4)
settings.SetInstanceDurationInDays(&instanceDurationInDays)
recurrence := msgraphsdk.NewPatternedRecurrence()
settings.SetRecurrence(recurrence)
pattern := msgraphsdk.NewRecurrencePattern()
recurrence.SetPattern(pattern)
type := "weekly"
pattern.SetType(&type)
interval := int32(1)
pattern.SetInterval(&interval)
range := msgraphsdk.NewRecurrenceRange()
recurrence.SetRange(range)
type := "noEnd"
range.SetType(&type)
startDate := "2020-09-08T12:02:30.667Z"
range.SetStartDate(&startDate)
decisionHistoriesForReviewersEnabled := true
settings.SetDecisionHistoriesForReviewersEnabled(&decisionHistoriesForReviewersEnabled)
result, err := graphClient.IdentityGovernance().AccessReviews().Definitions().Post(requestBody)


```