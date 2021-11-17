---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1f01cbff33423fd4f3189b3ebf8b7657324adb6
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61029010"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewEvent()
subject := "Plan summer company picnic"
requestBody.SetSubject(&subject)
body := msgraphsdk.NewItemBody()
requestBody.SetBody(body)
contentType := "HTML"
body.SetContentType(&contentType)
content := "Let's kick-start this event planning!"
body.SetContent(&content)
start := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetStart(start)
dateTime := "2017-08-30T11:00:00"
start.SetDateTime(&dateTime)
timeZone := "Pacific Standard Time"
start.SetTimeZone(&timeZone)
end := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetEnd(end)
dateTime := "2017-08-30T12:00:00"
end.SetDateTime(&dateTime)
timeZone := "Pacific Standard Time"
end.SetTimeZone(&timeZone)
requestBody.SetAttendees( []Attendee {
    msgraphsdk.NewAttendee(),
    SetAdditionalData(map[string]interface{}{
        "type": "Required",
    }
    msgraphsdk.NewAttendee(),
    SetAdditionalData(map[string]interface{}{
        "type": "Required",
    }
}
location := msgraphsdk.NewLocation()
requestBody.SetLocation(location)
displayName := "Conf Room 3; Fourth Coffee; Home Office"
location.SetDisplayName(&displayName)
locationType := "Default"
location.SetLocationType(&locationType)
requestBody.SetLocations( []Location {
    msgraphsdk.NewLocation(),
    SetAdditionalData(map[string]interface{}{
        "displayName": "Conf Room 3",
    }
    msgraphsdk.NewLocation(),
    SetAdditionalData(map[string]interface{}{
        "displayName": "Fourth Coffee",
    }
    msgraphsdk.NewLocation(),
    SetAdditionalData(map[string]interface{}{
        "displayName": "Home Office",
    }
}
allowNewTimeProposals := true
requestBody.SetAllowNewTimeProposals(&allowNewTimeProposals)
headers := map[string]string{
    "Prefer": "outlook.timezone="Pacific Standard Time""
}
options := &msgraphsdk.EventsRequestBuilderPostOptions{
    Body: requestBody,
    H: headers,
}
result, err := graphClient.Me().Events().Post(options)


```