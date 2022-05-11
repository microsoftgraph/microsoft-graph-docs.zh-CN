---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d12df7a00559cb2c9426630b0caf281c2230f56
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328180"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewSessionIdRequestBody()
sessionId := "22553876-f5ab-4529-bffb-cfe50aa89f87"
requestBody.SetSessionId(&sessionId)
userId := "user-id"
graphClient.UsersById(&userId).Presence().ClearPresence(user-id).Post(requestBody)


```