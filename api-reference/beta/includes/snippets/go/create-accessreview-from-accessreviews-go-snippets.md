---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a7f84c4180c5b9383fd15c769ad91f7f2f4f5066
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098663"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessReview()
displayName := "TestReview"
requestBody.SetDisplayName(&displayName)
startDateTime, err := time.Parse(time.RFC3339, "2017-02-10T00:35:53.214Z")
requestBody.SetStartDateTime(&startDateTime)
endDateTime, err := time.Parse(time.RFC3339, "2017-03-12T00:35:53.214Z")
requestBody.SetEndDateTime(&endDateTime)
reviewedEntity := msgraphsdk.NewIdentity()
requestBody.SetReviewedEntity(reviewedEntity)
id := "99025615-a0b1-47ec-9117-35377b10998b"
reviewedEntity.SetId(&id)
reviewerType := "delegated"
requestBody.SetReviewerType(&reviewerType)
businessFlowTemplateId := "6e4f3d20-c5c3-407f-9695-8460952bcc68"
requestBody.SetBusinessFlowTemplateId(&businessFlowTemplateId)
description := "Sample description"
requestBody.SetDescription(&description)
requestBody.SetReviewers( []AccessReviewReviewer {
    msgraphsdk.NewAccessReviewReviewer(),
id := "f260246a-09b1-4fd5-8d18-daed736071ec"
    SetId(&id)
    msgraphsdk.NewAccessReviewReviewer(),
id := "5a4e184c-4ee5-4883-96e9-b371f8da88e3"
    SetId(&id)
}
settings := msgraphsdk.NewAccessReviewSettings()
requestBody.SetSettings(settings)
mailNotificationsEnabled := true
settings.SetMailNotificationsEnabled(&mailNotificationsEnabled)
remindersEnabled := true
settings.SetRemindersEnabled(&remindersEnabled)
justificationRequiredOnApproval := true
settings.SetJustificationRequiredOnApproval(&justificationRequiredOnApproval)
autoReviewEnabled := false
settings.SetAutoReviewEnabled(&autoReviewEnabled)
activityDurationInDays := int32(30)
settings.SetActivityDurationInDays(&activityDurationInDays)
autoApplyReviewResultsEnabled := false
settings.SetAutoApplyReviewResultsEnabled(&autoApplyReviewResultsEnabled)
accessRecommendationsEnabled := false
settings.SetAccessRecommendationsEnabled(&accessRecommendationsEnabled)
recurrenceSettings := msgraphsdk.NewAccessReviewRecurrenceSettings()
settings.SetRecurrenceSettings(recurrenceSettings)
recurrenceType := "onetime"
recurrenceSettings.SetRecurrenceType(&recurrenceType)
recurrenceEndType := "endBy"
recurrenceSettings.SetRecurrenceEndType(&recurrenceEndType)
durationInDays := int32(0)
recurrenceSettings.SetDurationInDays(&durationInDays)
recurrenceCount := int32(0)
recurrenceSettings.SetRecurrenceCount(&recurrenceCount)
autoReviewSettings := msgraphsdk.NewAutoReviewSettings()
settings.SetAutoReviewSettings(autoReviewSettings)
notReviewedResult := "Deny"
autoReviewSettings.SetNotReviewedResult(&notReviewedResult)
result, err := graphClient.AccessReviews().Post(requestBody)


```