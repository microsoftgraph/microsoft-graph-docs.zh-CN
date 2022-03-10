---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d7da3d2dd0953344ae5b0a0e604de61f0cf4da0
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411787"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDestinationIdRequestBody()
destinationId := "destinationId-value"
requestBody.SetDestinationId(&destinationId)
options := &msgraphsdk.CopyRequestBuilderPostOptions{
    Body: requestBody,
}
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).Copy(message-id).Post(options)


```