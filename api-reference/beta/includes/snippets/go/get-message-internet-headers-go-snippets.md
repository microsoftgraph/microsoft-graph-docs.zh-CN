---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f05418c5bebaeae91fc9c26fa0e3b6b826146ab2
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097386"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.MessageRequestBuilderGetQueryParameters{
    Select: "internetMessageHeaders",
}
options := &msgraphsdk.MessageRequestBuilderGetOptions{
    Q: requestParameters,
}
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).Get(options)


```