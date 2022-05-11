---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7710120fe2735c490902c552e253b929f60c50be
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327334"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewNewReminderTimeRequestBody()
newReminderTime := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetNewReminderTime(newReminderTime)
dateTime := "dateTime-value"
newReminderTime.SetDateTime(&dateTime)
timeZone := "timeZone-value"
newReminderTime.SetTimeZone(&timeZone)
eventId := "event-id"
graphClient.Me().EventsById(&eventId).SnoozeReminder(event-id).Post(requestBody)


```