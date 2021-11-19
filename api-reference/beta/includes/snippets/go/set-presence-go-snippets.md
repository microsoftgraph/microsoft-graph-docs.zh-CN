---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b24da43b4340df9c4e34e50dfc15afb44906b43
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095751"
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
graphClient.UsersById(&userId).Presence().SetPresence().Post(options)


```