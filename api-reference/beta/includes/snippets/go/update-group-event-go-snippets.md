---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c8bc21e6ae536f65ebb47551c951faa508d8197c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61015131"
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
graphClient.GroupsById(&groupId).EventsById(&eventId).Patch(options)


```