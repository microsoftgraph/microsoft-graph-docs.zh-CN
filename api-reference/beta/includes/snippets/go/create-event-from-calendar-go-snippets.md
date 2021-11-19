---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9952932d0c1bb3ba4cf24926c088c5f996aa7cf0
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101526"
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
content := "Does next month work for you?"
body.SetContent(&content)
start := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetStart(start)
dateTime := "2019-03-10T12:00:00"
start.SetDateTime(&dateTime)
timeZone := "Pacific Standard Time"
start.SetTimeZone(&timeZone)
end := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetEnd(end)
dateTime := "2019-03-10T14:00:00"
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
options := &msgraphsdk.EventsRequestBuilderPostOptions{
    Body: requestBody,
}
calendarId := "calendar-id"
result, err := graphClient.Me().CalendarsById(&calendarId).Events().Post(options)


```