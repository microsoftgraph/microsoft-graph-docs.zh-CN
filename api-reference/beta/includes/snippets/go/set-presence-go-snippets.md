---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 999e83affbc09d8eb2663e3e4186506f84f77a70
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412715"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
sessionId := "22553876-f5ab-4529-bffb-cfe50aa89f87"
requestBody.SetSessionId(&sessionId)
availability := "Available"
requestBody.SetAvailability(&availability)
activity := "Available"
requestBody.SetActivity(&activity)
expirationDuration := "PT1H"
requestBody.SetExpirationDuration(&expirationDuration)
options := &msgraphsdk.SetPresenceRequestBuilderPostOptions{
    Body: requestBody,
}
userId := "user-id"
graphClient.UsersById(&userId).Presence().SetPresence(user-id).Post(options)


```