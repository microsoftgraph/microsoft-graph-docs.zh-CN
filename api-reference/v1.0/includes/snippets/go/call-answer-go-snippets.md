---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45b5b7963ab107e493664ecba4c32bd738823319
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326524"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
callbackUri := "callbackUri-value"
requestBody.SetCallbackUri(&callbackUri)
mediaConfig := msgraphsdk.NewMediaConfig()
requestBody.SetMediaConfig(mediaConfig)
mediaConfig.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<Media Session Configuration Blob>",
}
requestBody.SetAcceptedModalities( []Modality {
    "audio",
}
participantCapacity := int32(200)
requestBody.SetParticipantCapacity(&participantCapacity)
callId := "call-id"
graphClient.Communications().CallsById(&callId).Answer(call-id).Post(requestBody)


```