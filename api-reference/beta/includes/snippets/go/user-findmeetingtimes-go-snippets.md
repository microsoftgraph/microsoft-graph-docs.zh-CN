---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3aba89d549c8e16d35ef88f000deae8e8377b7b2
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096980"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAttendees( []AttendeeBase {
    msgraphsdk.NewAttendeeBase(),
    SetAdditionalData(map[string]interface{}{
        "type": "required",
    }
}
locationConstraint := msgraphsdk.NewLocationConstraint()
requestBody.SetLocationConstraint(locationConstraint)
isRequired := "false"
locationConstraint.SetIsRequired(&isRequired)
suggestLocation := "false"
locationConstraint.SetSuggestLocation(&suggestLocation)
locationConstraint.SetLocations( []LocationConstraintItem {
    msgraphsdk.NewLocationConstraintItem(),
    SetAdditionalData(map[string]interface{}{
        "resolveAvailability": "false",
        "displayName": "Conf room Hood",
    }
}
timeConstraint := msgraphsdk.NewTimeConstraint()
requestBody.SetTimeConstraint(timeConstraint)
activityDomain := "work"
timeConstraint.SetActivityDomain(&activityDomain)
timeConstraint.SetTimeSlots( []TimeSlot {
    msgraphsdk.NewTimeSlot(),
    SetAdditionalData(map[string]interface{}{
    }
}
isOrganizerOptional := "false"
requestBody.SetIsOrganizerOptional(&isOrganizerOptional)
meetingDuration := "PT1H"
requestBody.SetMeetingDuration(&meetingDuration)
returnSuggestionReasons := "true"
requestBody.SetReturnSuggestionReasons(&returnSuggestionReasons)
minimumAttendeePercentage := "100"
requestBody.SetMinimumAttendeePercentage(&minimumAttendeePercentage)
headers := map[string]string{
    "Prefer": "outlook.timezone="Pacific Standard Time""
}
options := &msgraphsdk.FindMeetingTimesRequestBuilderPostOptions{
    Body: requestBody,
    H: headers,
}
result, err := graphClient.Me().FindMeetingTimes().Post(options)


```