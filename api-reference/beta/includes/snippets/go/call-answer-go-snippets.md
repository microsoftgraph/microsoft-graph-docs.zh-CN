---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b6fa6d58c1e9aac3b2ba2bd9b5e933bb326e062
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220299"
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
options := &msgraphsdk.AnswerRequestBuilderPostOptions{
    Body: requestBody,
}
callId := "call-id"
graphClient.Communications().CallsById(&callId).Answer(call-id).Post(options)


```