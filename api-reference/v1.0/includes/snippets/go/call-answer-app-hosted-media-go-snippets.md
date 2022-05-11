---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7891557728ba5854ce241b115582366a318e5c7
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326523"
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
callId := "call-id"
graphClient.Communications().CallsById(&callId).Answer(call-id).Post(requestBody)


```