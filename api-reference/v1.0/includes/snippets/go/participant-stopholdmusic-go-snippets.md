---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c2a5d69012e0306534455682de4a6527c5812e7
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412194"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewClientContextRequestBody()
clientContext := "d45324c1-fcb5-430a-902c-f20af696537c"
requestBody.SetClientContext(&clientContext)
options := &msgraphsdk.StopHoldMusicRequestBuilderPostOptions{
    Body: requestBody,
}
callId := "call-id"
participantId := "participant-id"
result, err := graphClient.Communications().CallsById(&callId).ParticipantsById(&participantId).StopHoldMusic(call-id, participant-id).Post(options)


```