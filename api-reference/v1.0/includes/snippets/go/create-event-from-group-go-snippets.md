---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e22fbc323b674da1747a44048cb3198d1ab8aeb8
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327071"
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
content := "Does late morning work for you?"
body.SetContent(&content)
start := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetStart(start)
dateTime := "2019-06-16T12:00:00"
start.SetDateTime(&dateTime)
timeZone := "Pacific Standard Time"
start.SetTimeZone(&timeZone)
end := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetEnd(end)
dateTime := "2019-06-16T14:00:00"
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
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Events().Post(requestBody)


```