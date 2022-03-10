---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d214d57e573dfe71deeb36807923f885195287e
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412252"
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
uid := "iCalUId-value"
requestBody.SetUid(&uid)
reminderMinutesBeforeStart := int32(99)
requestBody.SetReminderMinutesBeforeStart(&reminderMinutesBeforeStart)
isReminderOn := true
requestBody.SetIsReminderOn(&isReminderOn)
options := &msgraphsdk.EventRequestBuilderPatchOptions{
    Body: requestBody,
}
groupId := "group-id"
eventId := "event-id"
result, err := graphClient.GroupsById(&groupId).EventsById(&eventId).Patch(options)


```