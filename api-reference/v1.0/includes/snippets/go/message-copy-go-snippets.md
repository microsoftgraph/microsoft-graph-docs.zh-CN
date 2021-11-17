---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 63d32f3684e0ae02ee2f6d056d6cecfe018afae2
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61027423"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
destinationId := "destinationId-value"
requestBody.SetDestinationId(&destinationId)
options := &msgraphsdk.CopyRequestBuilderPostOptions{
    Body: requestBody,
}
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).Copy().Post(options)


```