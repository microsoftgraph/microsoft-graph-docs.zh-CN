---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a029c615ac9172601eb462462be4d6e61ac49ee
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328184"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewClientContextRequestBody()
clientContext := "d45324c1-fcb5-430a-902c-f20af696537c"
requestBody.SetClientContext(&clientContext)
callId := "call-id"
participantId := "participant-id"
result, err := graphClient.Communications().CallsById(&callId).ParticipantsById(&participantId).Mute(call-id, participant-id).Post(requestBody)


```