---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 87ba287cf26acfe6914e77aa3469bad31bc7c029
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103567"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
destinationId := "deleteditems"
requestBody.SetDestinationId(&destinationId)
options := &msgraphsdk.MoveRequestBuilderPostOptions{
    Body: requestBody,
}
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).Move().Post(options)


```