---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94b39203053e0b8b49560f9db4e4e2a8246483fd
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60978917"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
iCalUId := "iCalUId-value"
requestBody.SetICalUId(&iCalUId)
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