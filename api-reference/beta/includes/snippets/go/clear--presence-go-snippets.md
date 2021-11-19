---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e7aa924cff8d6e245c694ca152b3d158aa81426c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100699"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
sessionId := "22553876-f5ab-4529-bffb-cfe50aa89f87"
requestBody.SetSessionId(&sessionId)
options := &msgraphsdk.ClearPresenceRequestBuilderPostOptions{
    Body: requestBody,
}
userId := "user-id"
graphClient.UsersById(&userId).Presence().ClearPresence().Post(options)


```