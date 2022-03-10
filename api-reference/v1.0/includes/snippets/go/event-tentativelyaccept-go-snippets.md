---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b314f23583ba5b90be0e190cebc81936c6f82c00
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411868"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
comment := "I may not be able to make this week. How about next week?"
requestBody.SetComment(&comment)
sendResponse := true
requestBody.SetSendResponse(&sendResponse)
proposedNewTime := msgraphsdk.NewTimeSlot()
requestBody.SetProposedNewTime(proposedNewTime)
start := msgraphsdk.NewDateTimeTimeZone()
proposedNewTime.SetStart(start)
dateTime := "2019-12-02T18:00:00"
start.SetDateTime(&dateTime)
timeZone := "Pacific Standard Time"
start.SetTimeZone(&timeZone)
end := msgraphsdk.NewDateTimeTimeZone()
proposedNewTime.SetEnd(end)
dateTime := "2019-12-02T19:00:00"
end.SetDateTime(&dateTime)
timeZone := "Pacific Standard Time"
end.SetTimeZone(&timeZone)
options := &msgraphsdk.TentativelyAcceptRequestBuilderPostOptions{
    Body: requestBody,
}
eventId := "event-id"
graphClient.Me().EventsById(&eventId).TentativelyAccept(event-id).Post(options)


```