---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d7d0cf8c59d96b479107f5e1c5f57e8efc344a5
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412033"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDestinationIdRequestBody()
destinationId := "deleteditems"
requestBody.SetDestinationId(&destinationId)
options := &msgraphsdk.MoveRequestBuilderPostOptions{
    Body: requestBody,
}
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).Move(message-id).Post(options)


```