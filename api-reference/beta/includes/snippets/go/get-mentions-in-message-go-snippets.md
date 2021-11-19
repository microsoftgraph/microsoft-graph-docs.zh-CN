---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 01cce4f12d9c1c554d4afe505c33a1b691ee666d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097574"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.MessageRequestBuilderGetQueryParameters{
    Expand: "mentions",
}
options := &msgraphsdk.MessageRequestBuilderGetOptions{
    Q: requestParameters,
}
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).Get(options)


```