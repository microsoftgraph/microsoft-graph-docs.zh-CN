---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 881742f7e0238929ee0fbc7192d9234de3b05892
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411921"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
callbackUri := "https://bot.contoso.com/api/calls"
requestBody.SetCallbackUri(&callbackUri)
requestBody.SetAcceptedModalities( []Modality {
    "audio",
}
mediaConfig := msgraphsdk.NewMediaConfig()
requestBody.SetMediaConfig(mediaConfig)
mediaConfig.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<Media Session Configuration Blob>",
}
options := &msgraphsdk.AnswerRequestBuilderPostOptions{
    Body: requestBody,
}
callId := "call-id"
graphClient.Communications().CallsById(&callId).Answer(call-id).Post(options)


```