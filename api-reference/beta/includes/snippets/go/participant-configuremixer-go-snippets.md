---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d4d3bcfb33fe86c60d2305372976382e4c3704d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328078"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
    "participantMixerLevels":  []Object {
    }
}
callId := "call-id"
participantId := "participant-id"
graphClient.Communications().CallsById(&callId).ParticipantsById(&participantId).Post(requestBody)


```