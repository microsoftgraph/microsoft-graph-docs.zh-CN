---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ece8bd201ba0ab329e59d0154ede573b18be5fa
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083800"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
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
graphClient.Me().EventsById(&eventId).SnoozeReminder().Post(options)


```