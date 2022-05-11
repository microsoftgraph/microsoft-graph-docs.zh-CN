---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c0db9899e8293e8c8286a1218c6b1bbedf1f5a8
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327697"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDestinationIdRequestBody()
destinationId := "deleteditems"
requestBody.SetDestinationId(&destinationId)
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).Move(message-id).Post(requestBody)


```