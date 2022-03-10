---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec83ff0b20e028f13e51727fa7596b0d99e57fc5
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412512"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewSessionIdRequestBody()
sessionId := "22553876-f5ab-4529-bffb-cfe50aa89f87"
requestBody.SetSessionId(&sessionId)
options := &msgraphsdk.ClearPresenceRequestBuilderPostOptions{
    Body: requestBody,
}
userId := "user-id"
graphClient.UsersById(&userId).Presence().ClearPresence(user-id).Post(options)


```