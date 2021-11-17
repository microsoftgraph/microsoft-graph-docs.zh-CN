---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb6fb386af15c250025d81304aebb937bf383cab
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60989679"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
graphClient.UsersById(&userId).Presence().SetPresence().Post(options)


```