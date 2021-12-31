---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e6a4d21be209343aef6bf7f4daa0350cba62d8c7
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61651565"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessReviewScheduleDefinition()
displayName := "Test create"
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
requestBody.SetReviewers( []AccessReviewReviewerScope {
    msgraphsdk.NewAccessReviewReviewerScope(),
    SetAdditionalData(map[string]interface{}{
        "query": "/users/398164b1-5196-49dd-ada2-364b49f99b27",
        "queryType": "MicrosoftGraph",
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
instanceDurationInDays := int32(1)
settings.SetInstanceDurationInDays(&instanceDurationInDays)
recommendationsEnabled := true
settings.SetRecommendationsEnabled(&recommendationsEnabled)
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
options := &msgraphsdk.DefinitionsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.IdentityGovernance().AccessReviews().Definitions().Post(options)


```