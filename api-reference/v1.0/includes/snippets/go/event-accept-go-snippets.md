---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b6e6e8a67f4681fd42f7b6ed2f61d6afe0563d1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328328"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
comment := "comment-value"
requestBody.SetComment(&comment)
sendResponse := true
requestBody.SetSendResponse(&sendResponse)
eventId := "event-id"
graphClient.Me().EventsById(&eventId).Accept(event-id).Post(requestBody)


```