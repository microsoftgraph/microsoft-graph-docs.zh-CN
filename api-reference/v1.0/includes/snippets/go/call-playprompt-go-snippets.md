---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bdaa484e2a99ac39788363eb2042b007ed532ad3
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61006984"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
result, err := graphClient.Communications().CallsById(&callId).PlayPrompt().Post(options)


```