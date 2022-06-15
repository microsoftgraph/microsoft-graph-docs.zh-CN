---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b5bbf0253ba27c8855fc8d77c989d98797d82edd
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098786"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTimeCard()
clockInEvent := msgraphsdk.NewTimeCardEvent()
requestBody.SetClockInEvent(clockInEvent)
dateTime, err := time.Parse(time.RFC3339, "2019-03-18T00:00:00.000Z")
clockInEvent.SetDateTime(&dateTime)
atApprovedLocation := true
clockInEvent.SetAtApprovedLocation(&atApprovedLocation)
notes := msgraphsdk.NewItemBody()
clockInEvent.SetNotes(notes)
content := "Started late due to traffic in CA 237"
notes.SetContent(&content)
contentType := "text"
notes.SetContentType(&contentType)
notes := msgraphsdk.NewItemBody()
requestBody.SetNotes(notes)
content := "8 To 5 Inventory management"
notes.SetContent(&content)
contentType := "text"
notes.SetContentType(&contentType)
requestBody.SetBreaks( []TimeCardBreak {
    msgraphsdk.NewTimeCardBreak(),
breakId := "string"
    SetBreakId(&breakId)
notes := msgraphsdk.NewItemBody()
    SetNotes(notes)
content := "Lunch break"
    notes.SetContent(&content)
contentType := "text"
    notes.SetContentType(&contentType)
start := msgraphsdk.NewTimeCardEvent()
    SetStart(start)
dateTime, err := time.Parse(time.RFC3339, "2019-03-18T02:00:00.000Z")
    start.SetDateTime(&dateTime)
atApprovedLocation := true
    start.SetAtApprovedLocation(&atApprovedLocation)
notes := msgraphsdk.NewItemBody()
    start.SetNotes(notes)
content := "Reduced break to make up for lost time"
    notes.SetContent(&content)
contentType := "text"
    notes.SetContentType(&contentType)
}
requestBody.SetAdditionalData(map[string]interface{}{
    "onBehalfOfUserId": "a3601044-a1b5-438e-b742-f78d01d68a67",
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Schedule().TimeCards().Post(requestBody)


```