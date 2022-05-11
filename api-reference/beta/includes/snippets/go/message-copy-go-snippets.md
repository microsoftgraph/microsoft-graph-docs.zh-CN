---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92f380cfc897a0cc1e72f67eb787983fa56e4839
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328081"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDestinationIdRequestBody()
destinationId := "destinationId-value"
requestBody.SetDestinationId(&destinationId)
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).Copy(message-id).Post(requestBody)


```