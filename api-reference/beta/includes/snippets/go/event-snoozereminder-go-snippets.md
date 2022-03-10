---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3bbb55eba15de4c3420959e57c112e694474cb9
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412039"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewNewReminderTimeRequestBody()
newReminderTime := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetNewReminderTime(newReminderTime)
dateTime := "2016-10-19T10:37:00Z"
newReminderTime.SetDateTime(&dateTime)
timeZone := "timeZone-value"
newReminderTime.SetTimeZone(&timeZone)
options := &msgraphsdk.SnoozeReminderRequestBuilderPostOptions{
    Body: requestBody,
}
eventId := "event-id"
graphClient.Me().EventsById(&eventId).SnoozeReminder(event-id).Post(options)


```