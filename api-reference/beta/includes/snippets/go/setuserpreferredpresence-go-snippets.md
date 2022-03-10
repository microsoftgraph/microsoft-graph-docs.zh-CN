---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5155414adc890b457f5b9c5fe50c7bab32d4d274
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412031"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
availability := "DoNotDisturb"
requestBody.SetAvailability(&availability)
activity := "DoNotDisturb"
requestBody.SetActivity(&activity)
expirationDuration := "PT8H"
requestBody.SetExpirationDuration(&expirationDuration)
options := &msgraphsdk.SetUserPreferredPresenceRequestBuilderPostOptions{
    Body: requestBody,
}
userId := "user-id"
graphClient.UsersById(&userId).Presence().SetUserPreferredPresence(user-id).Post(options)


```