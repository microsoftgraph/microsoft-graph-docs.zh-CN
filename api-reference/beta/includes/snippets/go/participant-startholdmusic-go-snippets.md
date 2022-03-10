---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce917a189fc31d485429dfde8bbd9ff7a6b3db32
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412548"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
customPrompt := msgraphsdk.NewPrompt()
requestBody.SetCustomPrompt(customPrompt)
customPrompt.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.mediaPrompt",
}
clientContext := "d45324c1-fcb5-430a-902c-f20af696537c"
requestBody.SetClientContext(&clientContext)
options := &msgraphsdk.StartHoldMusicRequestBuilderPostOptions{
    Body: requestBody,
}
callId := "call-id"
participantId := "participant-id"
result, err := graphClient.Communications().CallsById(&callId).ParticipantsById(&participantId).StartHoldMusic(call-id, participant-id).Post(options)


```