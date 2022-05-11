---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 853bff74f0051d38bf4a31a9f4f32053b896c3f9
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328267"
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
callOptions := msgraphsdk.NewIncomingCallOptions()
requestBody.SetCallOptions(callOptions)
isContentSharingNotificationEnabled := true
callOptions.SetIsContentSharingNotificationEnabled(&isContentSharingNotificationEnabled)
callOptions.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.incomingCallOptions",
}
participantCapacity := int32(200)
requestBody.SetParticipantCapacity(&participantCapacity)
callId := "call-id"
graphClient.Communications().CallsById(&callId).Answer(call-id).Post(requestBody)


```