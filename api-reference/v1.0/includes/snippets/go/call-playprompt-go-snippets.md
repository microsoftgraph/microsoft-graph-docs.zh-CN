---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce1858b076354be33751c9469906908043cb8c6a
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412529"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
clientContext := "d45324c1-fcb5-430a-902c-f20af696537c"
requestBody.SetClientContext(&clientContext)
requestBody.SetPrompts( []Prompt {
    msgraphsdk.NewPrompt(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.mediaPrompt",
    }
}
options := &msgraphsdk.PlayPromptRequestBuilderPostOptions{
    Body: requestBody,
}
callId := "call-id"
result, err := graphClient.Communications().CallsById(&callId).PlayPrompt(call-id).Post(options)


```