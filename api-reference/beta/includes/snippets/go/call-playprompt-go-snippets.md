---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2d5e12583a7495a1ff5ad4a472178361da7bb90
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137706"
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
loop := false
requestBody.SetLoop(&loop)
options := &msgraphsdk.PlayPromptRequestBuilderPostOptions{
    Body: requestBody,
}
callId := "call-id"
result, err := graphClient.Communications().CallsById(&callId).PlayPrompt().Post(options)


```