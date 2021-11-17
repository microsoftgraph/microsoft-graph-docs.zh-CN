---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37113970b67b993c5338ab5cdc0536e687c53616
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60993227"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
comment := "I won't be able to make this week. How about next week?"
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
options := &msgraphsdk.DeclineRequestBuilderPostOptions{
    Body: requestBody,
}
eventId := "event-id"
graphClient.Me().EventsById(&eventId).Decline().Post(options)


```