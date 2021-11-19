---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eefd2374ef9a486f0b54ae10687f05fefab600ee
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085547"
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
options := &msgraphsdk.AnswerRequestBuilderPostOptions{
    Body: requestBody,
}
callId := "call-id"
graphClient.Communications().CallsById(&callId).Answer().Post(options)


```