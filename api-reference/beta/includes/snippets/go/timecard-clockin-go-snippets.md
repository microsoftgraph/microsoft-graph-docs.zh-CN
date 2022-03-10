---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6809d630fb17d6772b822277c38876190b55a3a
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412604"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
notes := msgraphsdk.NewItemBody()
requestBody.SetNotes(notes)
contentType := "text"
notes.SetContentType(&contentType)
content := "clock in notes"
notes.SetContent(&content)
requestBody.SetAdditionalData(map[string]interface{}{
    "atAprovedLocation": true,
}
options := &msgraphsdk.ClockInRequestBuilderPostOptions{
    Body: requestBody,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Schedule().TimeCards().ClockIn(team-id).Post(options)


```