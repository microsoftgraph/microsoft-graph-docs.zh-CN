---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5175a4bc6a1e66b7fcb5b1f4e931cf14aa28cce3
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099710"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
comment := "comment-value"
requestBody.SetComment(&comment)
sendResponse := true
requestBody.SetSendResponse(&sendResponse)
options := &msgraphsdk.AcceptRequestBuilderPostOptions{
    Body: requestBody,
}
eventId := "event-id"
graphClient.Me().EventsById(&eventId).Accept().Post(options)


```