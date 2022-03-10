---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00391a153fa7835b9c1b4199ea2ad94879205710
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411880"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
bargeInAllowed := true
requestBody.SetBargeInAllowed(&bargeInAllowed)
clientContext := "d45324c1-fcb5-430a-902c-f20af696537c"
requestBody.SetClientContext(&clientContext)
requestBody.SetPrompts( []Prompt {
    msgraphsdk.NewPrompt(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.mediaPrompt",
    }
}
maxRecordDurationInSeconds := int32(10)
requestBody.SetMaxRecordDurationInSeconds(&maxRecordDurationInSeconds)
initialSilenceTimeoutInSeconds := int32(5)
requestBody.SetInitialSilenceTimeoutInSeconds(&initialSilenceTimeoutInSeconds)
maxSilenceTimeoutInSeconds := int32(2)
requestBody.SetMaxSilenceTimeoutInSeconds(&maxSilenceTimeoutInSeconds)
playBeep := true
requestBody.SetPlayBeep(&playBeep)
requestBody.SetStopTones( []String {
    "#",
    "1",
    "*",
}
options := &msgraphsdk.RecordResponseRequestBuilderPostOptions{
    Body: requestBody,
}
callId := "call-id"
result, err := graphClient.Communications().CallsById(&callId).RecordResponse(call-id).Post(options)


```