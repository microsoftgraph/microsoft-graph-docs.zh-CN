---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 401f18d80757c5358ba1bb45af94a3330dfde784
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129288"
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
    SetAdditionalData(map[string]interface{}{
        "breakId": "string",
    }
}
requestBody.SetAdditionalData(map[string]interface{}{
    "onBehalfOfUserId": "a3601044-a1b5-438e-b742-f78d01d68a67",
}
options := &msgraphsdk.TimeCardsRequestBuilderPostOptions{
    Body: requestBody,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Schedule().TimeCards().Post(options)


```