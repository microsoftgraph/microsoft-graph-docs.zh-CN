---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80979062869cf1891ec07d449aff9915f24414d4
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61228322"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEvent()
originalStartTimeZone := "originalStartTimeZone-value"
requestBody.SetOriginalStartTimeZone(&originalStartTimeZone)
originalEndTimeZone := "originalEndTimeZone-value"
requestBody.SetOriginalEndTimeZone(&originalEndTimeZone)
responseStatus := msgraphsdk.NewResponseStatus()
requestBody.SetResponseStatus(responseStatus)
response := ""
responseStatus.SetResponse(&response)
time, err := time.Parse(time.RFC3339, "datetime-value")
responseStatus.SetTime(&time)
requestBody.SetRecurrence(nil)
reminderMinutesBeforeStart := int32(99)
requestBody.SetReminderMinutesBeforeStart(&reminderMinutesBeforeStart)
isOnlineMeeting := true
requestBody.SetIsOnlineMeeting(&isOnlineMeeting)
onlineMeetingProvider := "teamsForBusiness"
requestBody.SetOnlineMeetingProvider(&onlineMeetingProvider)
isReminderOn := true
requestBody.SetIsReminderOn(&isReminderOn)
hideAttendees := false
requestBody.SetHideAttendees(&hideAttendees)
requestBody.SetCategories( []String {
    "Red category",
}
options := &msgraphsdk.EventRequestBuilderPatchOptions{
    Body: requestBody,
}
eventId := "event-id"
graphClient.Me().EventsById(&eventId).Patch(options)


```