---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d39c28877f81889c9c14a05124130fea45efeb56
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412709"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
notes := msgraphsdk.NewItemBody()
requestBody.SetNotes(notes)
contentType := "text"
notes.SetContentType(&contentType)
content := "end break smaple notes"
notes.SetContent(&content)
requestBody.SetAdditionalData(map[string]interface{}{
    "atAprovedLocation": true,
}
options := &msgraphsdk.EndBreakRequestBuilderPostOptions{
    Body: requestBody,
}
teamId := "team-id"
timeCardId := "timeCard-id"
result, err := graphClient.TeamsById(&teamId).Schedule().TimeCardsById(&timeCardId).EndBreak(team-id, timeCard-id).Post(options)


```