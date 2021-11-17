---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 924af592c8d661a857c873a1050fd32f7baa6262
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60988930"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
notes := msgraphsdk.NewItemBody()
requestBody.SetNotes(notes)
contentType := "text"
notes.SetContentType(&contentType)
content := "start break smaple notes"
notes.SetContent(&content)
requestBody.SetAdditionalData(map[string]interface{}{
    "atAprovedLocation": true,
}
options := &msgraphsdk.StartBreakRequestBuilderPostOptions{
    Body: requestBody,
}
teamId := "team-id"
timeCardId := "timeCard-id"
result, err := graphClient.TeamsById(&teamId).Schedule().TimeCardsById(&timeCardId).StartBreak().Post(options)


```