---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42b64de901be95350e16e9893e8844bdb7da60d5
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526093"
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
graphClient.UsersById(&userId).Presence().SetUserPreferredPresence().Post(options)


```