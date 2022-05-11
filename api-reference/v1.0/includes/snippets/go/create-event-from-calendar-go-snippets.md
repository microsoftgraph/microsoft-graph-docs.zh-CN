---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f82af5ab5b50c42705b8dab46624fef52025a66
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327523"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEvent()
subject := "Let's go for lunch"
requestBody.SetSubject(&subject)
body := msgraphsdk.NewItemBody()
requestBody.SetBody(body)
contentType := "HTML"
body.SetContentType(&contentType)
content := "Does mid month work for you?"
body.SetContent(&content)
start := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetStart(start)
dateTime := "2019-03-15T12:00:00"
start.SetDateTime(&dateTime)
timeZone := "Pacific Standard Time"
start.SetTimeZone(&timeZone)
end := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetEnd(end)
dateTime := "2019-03-15T14:00:00"
end.SetDateTime(&dateTime)
timeZone := "Pacific Standard Time"
end.SetTimeZone(&timeZone)
location := msgraphsdk.NewLocation()
requestBody.SetLocation(location)
displayName := "Harry's Bar"
location.SetDisplayName(&displayName)
requestBody.SetAttendees( []Attendee {
    msgraphsdk.NewAttendee(),
    SetAdditionalData(map[string]interface{}{
        "type": "required",
    }
}
transactionId := "7E163156-7762-4BEB-A1C6-729EA81755A7"
requestBody.SetTransactionId(&transactionId)
calendarId := "calendar-id"
result, err := graphClient.Me().CalendarsById(&calendarId).Events().Post(requestBody)


```